# Semaforo-IFA

### Códigos

#define Led_Vermelho 4
#define Led_Amarelo 3
#define Led_Verde 2

void setup()
{
  pinMode (Led_Vermelho, OUTPUT);
 
  pinMode (Led_Amarelo, OUTPUT);
  
  pinMode (Led_Verde, OUTPUT);
  
}

void loop()
           
{ digitalWrite (Led_Verde, HIGH); 
  digitalWrite (Led_Amarelo, LOW);
  digitalWrite (Led_Vermelho, LOW);
  delay (5000);
  
    
  digitalWrite (Led_Verde, LOW); 
  digitalWrite (Led_Amarelo, HIGH);
  digitalWrite (Led_Vermelho, LOW);
  delay (2000);
    
    
  digitalWrite (Led_Verde, LOW); 
  digitalWrite (Led_Amarelo, LOW);
  digitalWrite (Led_Vermelho, HIGH);
  delay (2000);
    
}
