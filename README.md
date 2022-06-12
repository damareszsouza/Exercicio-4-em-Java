# Exercicio-4-em-Java

# Exercicio replicado do Livro Tutorial de Programação em Java e Orientação a Objetos 
 
#  Método move:
# O método move altera as coordenadas do objeto. O objeto tem suas coordenadas x e y somadas
# com os argumentos dessa função. Note que este método representa uma maneira mais segura, clara,
# elegante de alterar as coordenadas do objeto do que acessá-las diretamente da seguinte forma: ac.x
# += dx;. ac.y += dy;. Lembre-se que ac.x += dx é uma abreviação para ac.x = ac.x+dx;. 
# Método mostra:
# O método mostra imprime na tela, de forma compacta, os atributos do objeto.

//Classe circulo
public class Circulo {
public float raio;
public float x;
//posicoes em coordenadas cartesianas
public float y;
public void move(float dx,float dy) { //move o circulo de lugar this.x += dx;
 y += dy;
}
public void mostra()
//imprime na tela estado do objeto
{
System.out.println("(" + x + "," + y + "," + raio + ")");
}
} //fim da declaracao da classe

//Classe principal, Arquivo Principal.Java
class Principal {
 public static void main(String args[]) {
 Circulo umcirc; 
 //declaracao de atributo circulo
 umcirc = new Circulo();
 umcirc.x = 0;
 umcirc.y = 0;
 umcirc.raio = 12;
 umcirc.mostra();
 umcirc.move(10,10);
 umcirc.mostra();
 umcirc.x = 100;
 umcirc.mostra();
 }
}
