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



## 2 Semaforo  cruzamento carros

/* Define as portas dos LED’s do semáforo 1 */
#define LED_Vermelho_1 4
#define LED_Amarelo_1 3
#define LED_Verde_1 2
/* Define as portas dos LED’s do semáforo 2 */
#define LED_Vermelho_2 7
#define LED_Amarelo_2 6
#define LED_Verde_2 5
/* Define todos os pinos dos LED’s como SAÍDA */
void setup() {
pinMode(LED_Vermelho_1, OUTPUT);
pinMode(LED_Amarelo_1, OUTPUT);
pinMode(LED_Verde_1, OUTPUT);
pinMode(LED_Vermelho_2, OUTPUT);
pinMode(LED_Amarelo_2, OUTPUT);
pinMode(LED_Verde_2, OUTPUT);
}
void loop() {
/* Primeiro estágio: Semáforo 1 ABERTO e Semáforo 2 FECHADO
(5 segundos) */
digitalWrite(LED_Vermelho_1, LOW);
digitalWrite(LED_Amarelo_1, LOW);
digitalWrite(LED_Verde_1, HIGH);
digitalWrite(LED_Vermelho_2, HIGH);
digitalWrite(LED_Amarelo_2, LOW);
digitalWrite(LED_Verde_2, LOW);
delay(5000);
/* Segundo estágio: Semáforo 1 ATENÇÃO E Semáforo 2 FECHADO
(3 segundos) */
digitalWrite(LED_Vermelho_1, LOW);
digitalWrite(LED_Amarelo_1, HIGH);
digitalWrite(LED_Verde_1, LOW);
digitalWrite(LED_Vermelho_2, HIGH);
digitalWrite(LED_Amarelo_2, LOW);
digitalWrite(LED_Verde_2, LOW);
delay(3000);
/* Terceiro estágio: Semáforo 1 Fechado e Semáforo 2 Aberto
(5 segundos) */
digitalWrite(LED_Vermelho_1, HIGH);
digitalWrite(LED_Amarelo_1, LOW);
digitalWrite(LED_Verde_1, LOW);
digitalWrite(LED_Vermelho_2, LOW);
digitalWrite(LED_Amarelo_2, LOW);
digitalWrite(LED_Verde_2, HIGH);
delay(5000);
/* Quarto estágio: Semáforo 1 FECHADO e Semáforo 2
ATENÇÃO (3 segundos) */
digitalWrite(LED_Vermelho_1, HIGH);
digitalWrite(LED_Amarelo_1, LOW);
digitalWrite(LED_Verde_1, LOW);
digitalWrite(LED_Vermelho_2, LOW);
digitalWrite(LED_Amarelo_2, HIGH);
digitalWrite(LED_Verde_2, LOW);
delay(3000);
}
