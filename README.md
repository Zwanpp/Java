# Java
package ControleEspaço;

import java.util.ArrayList;

public class Relatorio {

private double espaçoMedio;
private double espaçoTotal;
public Relatorio() {

}
public double getEspaçoMedio() {
	return espaçoMedio;
}
public void setEspaçoMedio(double espaçoMedio) {
	this.espaçoMedio = espaçoMedio;
}
public double getEspaçoTotal() {
	return espaçoTotal;
}
public void setEspaçoTotal(double espaçoTotal) {
	this.espaçoTotal = espaçoTotal;
}
	
	public void gerarRelatorio() {


     ArrayList<EspacoDisco> espaco = new ArrayList<EspacoDisco>();


     
	espaco.add(new EspacoDisco("alexandre",456123789));
	espaco.add(new EspacoDisco("anderson ",1245698456));
	espaco.add(new EspacoDisco("antonio",123456456));
	espaco.add(new EspacoDisco("carlos ",91257581));
	espaco.add(new EspacoDisco("cesar",987458));
	espaco.add(new EspacoDisco("rosemary",789456125));
	
	ArrayList<Double> espacoFinal = new ArrayList<Double>();
	
	espacoFinal.add((espaco.get(0).getEspaço())/ (1024*1024));
	espacoFinal.add((espaco.get(1).getEspaço())/ (1024*1024));
	espacoFinal.add((espaco.get(2).getEspaço())/ (1024*1024));
	espacoFinal.add((espaco.get(3).getEspaço())/ (1024*1024));
	espacoFinal.add((espaco.get(4).getEspaço())/ (1024*1024));
	espacoFinal.add((espaco.get(5).getEspaço())/ (1024*1024));

	for (int i = 0; i < espacoFinal.size(); i++) {
		espacoFinal.get(i);
		
	System.out.println(espacoFinal);	
	
	
	
	System.out.println(espaco.get(i).getNome());
	
	
	
	}
	package ControleEspaço;

public class MainRelatorio {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		 
		Relatorio conta = new Relatorio();
		
		conta.gerarRelatorio();
		
		
