
public interface ReprodutorMusical {

	public void tocar();
	public void pausar();
	public void selecionarMusica(String musica);}

public interface AparelhoTelefonico {

	public void ligar(String numero);
	public void atender();
	public void iniciarCorreioVoz();}
 
public interface NavegadorInternet {

	public void exibirPagina(String url);
	public void adicionarNovaAba();
	public void atualizarPagina();}

public class Iphone implements ReprodutorMusical, AparelhoTelefonico, NavegadorInternet {

	@Override
	public void exibirPagina(String url) {
		System.out.println("Exibindo a página: " + url);
	}

	@Override
	public void adicionarNovaAba() {
		System.out.println("Adicionando uma nova aba.");
	}

	@Override
	public void atualizarPagina() {
		System.out.println("Atualizando a página...");
	}

	@Override
	public void ligar(String numero) {
		System.out.println("Ligando para o número: " + numero);
		
	}

	@Override
	public void atender() {
		System.out.println("Atendendo a ligação.");
	}

	@Override
	public void iniciarCorreioVoz() {
		System.out.println("Abrindo o correio de voz.");
	}

	@Override
	public void tocar() {
		System.out.println("Tocando música");
	}

	@Override
	public void pausar() {
		System.out.println("Música pausada");
	}

	@Override
	public void selecionarMusica(String musica) {
		System.out.println("Selecionando a música: " + musica);
	}

	public static void main(String[] args) {
		Iphone meuIphone = new Iphone();
		
		meuIphone.tocar();
		meuIphone.ligar("222-5678");
		meuIphone.exibirPagina("www.google.com.br");
	}}
		
