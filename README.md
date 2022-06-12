# TP3DIEGO NEGRETE 1740229/ROBERTO RODRIGUES CB3000419
pacote tp03;

importação de java estático. Lang. O sistema. para um;
importação java. Util. Scanner;

classe pública Hora {
estática privada int hora, min, seg;
varredura scanner privada = novo Scanner (Sistema).

Hora pública(){
    int h,m, s ;
    
    tentar{
        fazer {
            para fora. impressão("Informe a hora: ");
            h = digitalização. nextInt();
        } enquanto (h < 0 || h > 23);
        
        fazer {
            para fora. imprimir("Informe os minutos: ");
            m = digitalização. nextInt();
        } enquanto (h < 0 || h > 59);
        
        fazer {
            para fora. imprimir("Informe os segundos: ");
            s = digitalização. nextInt();
        } enquanto (h < 0 || h > 59);
        
        nova Hora(h, m, s);
    }
    captura (Exceção e){
        para fora. println ("Erro\n" + e. getMessage());
    }
}

hora pública (int h, int m, int s){
    setHora(h));
    setMin(m));
    setSeg(s));
}

público int getHora() {
    hora de retorno ;
}

vazio público  setHora (int h) {
    hora = h;
}

público int getMin() {
    retorno min;
}

vazio público  setMin (int m) {
    min = m;
}

public int getSeg() {
    return seg;
}

public void setSeg(int s) {
    seg = s;
}

string público getHora1(){
    String ret = getHora() + + getMin() + ":" + getSeg();
    
    retorno ret;
}

string público getHora2(){
     Ret de cordas;
    
    se (getHora() < 12 && getHora() > 0)
        ret = getHora1() + " AM";
    mais{
        se (getHora() == 0)
            ret = ("12:" + getMin() + + getSeg() + " AM");
        mais{
             se (getHora() == 12)
                 ret = ("12:" + getMin() + + getSeg() + " PM");
             mais
                 ret = ((getHora() - 12) + + getMin() + + getSeg() + " PM");
        }                
    }
    
    retorno ret;
}

int público  getSegundos(){
    int ret;
    
    ret = getHora() * 60 * 60 + getMin() * 60 + getSeg();
    
    retorno ret;
}    
}
