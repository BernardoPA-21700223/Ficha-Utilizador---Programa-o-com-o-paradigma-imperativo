<div class="alert alert-info">
    <h2>Ficha Utilizador - Programação com o paradigma imperativo</h2>
    <p><strong><br>Introdução</strong></p>
    <p>Esta ficha destina-se à análise e à implementação de classes para representar uma realidade que se descreve de seguida.</p>
    <p>Mais concretamente, iremos implementar várias funções <code>static</code> que manipulam dados de objectos de uma classe. O que vamos fazer, 
	em termos práticos, é programação imperativa, usando classes como se fossem "estruturas".
    </p><p>Num determindo sistema, um utilizador é caracterizado por:
	</p><ul>
		<li>Primeiro nome</li>
		<li>Último nome</li>
		<li>E-mail</li>
		<li>Username</li>
		<li>Password</li>
	</ul>
    <p>O sistema tem uma componente de autenticação. Esta componente tem uma regra: se for falhada a autenticação de um dado utilizador mais do que 3 vezes seguidas, 
	esse utilizador fica bloqueado.
    </p><p><strong><br>Intruções</strong></p>
    <ol>
	<li>
		<p>Implemente a classe <code>Utilizador</code>, e adicione à mesma os atributos (variáveis) necessários para representar a informação descrita anteriormente.
	</p></li>
	<li>
		<p>Adicione à classe quatro construtores:
			</p><ul>
				<li>Um sem argumentos</li>
				<!--
				<li>Um que receba 1 String com o nome completo (vários nomes separados por um espaço em branco). Apenas o primeiro e último nomes devem ser considerados. 
				<p>Por exemplo, se for passada a String for "Ricardo Araújo Pereira", então o primeiro nome do utilizador será "Ricardo" e o último nome será "Pereira".
				Será garantido que serão sempre passados pelo menos 2 nomes.-->
				<li>Um que receba os 2 nomes como argumentos (os restantes devem ser deixados vazios/null)</li>
				<li>Um que receba os valores dos 5 atributos como argumentos (pela ordem do enunciado)</li>
			</ul>
	</li>
        <li>
            <p>Crie a classe <code>Main</code>, num ficheiro <code>Main.java</code>, e adicione à mesma a função <code>
                public static void main(String[] args)</code>.</p>
        </li>
        <li>
            <p>Implemente, na classe <code>Main</code>, estas funções:</p>
            <ol>
                <li>
			<code>static ArrayList&lt;Utilizador&gt; utilizadoresDoSistema()</code> - deve devolver um <code>ArrayList</code> com 4 objectos Utilizador. 
			<p>Cada objecto deve ser criado com um construtor diferente.
			</p><p>Apesar de o construtor vazio não receber argumentos, o objecto criado com o mesmo tem de ter valores para o primeiro nome e último nome.
			</p><p>Os dados de cada Utilizador ficam ao seu critério.
		</p></li>
		<li>
			<code>static String imprimirUtilizador(Utilizador obj)</code> - deve retornar uma String que contenha os dados do utilizador passado como argumento, usando a sintaxe seguinte:
				<code>"&lt;Primeiro nome&gt; &lt;Último nome&gt; (&lt;E-mail&gt; &lt;Username&gt;)"</code>
		</li>
		<li>
			<code>static ____ temEmail(Utilizador obj)</code> - deve devolver <code>true</code> caso o Utilizador passado como argumento tenha e-mail definido e <code>false</code> em caso contrário.
			<b>Dica:</b> Cuidado com null e com Strings vazias. <b>Desafio:</b> tenta resolver este exercício sem usar o <code>if</code>.
		</li>
		<li>
			<code>static ____ autenticar(Utilizador obj, String password)</code> - deve devolver <code>true</code> caso Utilizador passado como argumento tenha como password o segundo valor passado como argumento.
			Em caso contrário, deve devolver <code>false</code>.
			<p>Se o utilizador estiver "bloqueado", então esta função deve devolver false, independentemente da password estar certa ou errada.
			</p><p>Caso a autenticação deste Utilizador falhe mais do que 3 vezes seguidas, o mesmo deve passar a ser considerado como estando bloqueado.
		</p></li>
		<li>
			<code>static ____ utilizadorBloqueado(Utilizador obj)</code> - deve devolver true caso o Utilizador passado como argumento esteja bloqueado. Em caso contrário, deve devolver false.
		</li>
		<li>
			<code>static void desbloquearUtilizador(Utilizador obj)</code> - deve desbloquear o Utilizador passado como argumento.
		</li>
		<li>
			<code>static ____ temPasswordFraca(Utilizador obj)</code> - deve devolver true caso o Utilizador passado como argumento tenha uma password considerada fraca.
			<p>Uma password é considerada fraca se:
			</p><ol>
				<li>for null</li>
				<li>tiver menos de 6 caracteres</li>
				<li>tive apenas letras ou apenas números</li>
			</ol>
			<b>Dicas</b>: podem ser uteis as funções <code>Character.isLetter()</code> e <code>Character.isDigit()</code>. Exemplos: as chamadas <code>Character.isLetter('A')</code> e <code>Character.isDigit('1')</code> vão retornar ambas true.
		</li>
		<li>
			<code>static ____ emailExistente(ArrayList&lt;Utilizador&gt; utilizadores, String email)</code> - deve retornar <code>true</code> caso exista um utilizador que tenha 
			o <code>email</code> passado como argumento. Em caso contrário, deve devolver <code>false</code>.
		</li>
		<li>
			<code>static ArrayList&lt;String&gt; obterEmails(ArrayList&lt;Utilizador&gt; utilizadores)</code> - deve devolver os e-mails de todos os utilizadores. A ordem é irrelevante.
		</li>
            </ol>
        </li>
    </ol>
    <p><strong><br>Notas</strong></p>
    <p>Tenha o cuidado de respeitar os nomes, tipos de dados e formatos indicados</p>
</div>
