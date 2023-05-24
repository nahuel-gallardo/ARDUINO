# SISTEMA DE PROCESAMIENTO DE DATOS.UTN

 
____________________________________________________________________________________________________________
INTEGRANTES
NAHUEL IAIR GALLARDO

______________________________________________________________________________________________
PORYECTO : MONTACARGA

 

Descripción
___________________________________________________________________________________________________________________

modelo de montacarga funcional como maqueta para un hospital.
recibe ordenes de subir, bajar o pausar desde diferentes pisos 

Función principal
___________________________________________________________________________________________________________________

 if(presiono_1 == 1)
    {
      
      digitalWrite(LED_VERDE,HIGH);
      digitalWrite(ENTRADA_1,HIGH);
      digitalWrite(ENTRADA_2,LOW);
      piso = 1;
      delay(3000);
      digitalWrite(LED_VERDE,LOW);
      digitalWrite(ENTRADA_1,LOW);
      digitalWrite(ENTRADA_2,LOW);
      acumulador = acumulador + (piso);
    }

    if(presiono_2 == 1)
    {
      digitalWrite(LED_VERDE,HIGH);
      digitalWrite(ENTRADA_1,LOW);
      digitalWrite(ENTRADA_2,HIGH);
      piso = -1;
      delay(3000);
      digitalWrite(LED_VERDE,LOW);
      digitalWrite(ENTRADA_1,LOW);
      digitalWrite(ENTRADA_2,LOW);
      acumulador = acumulador + (piso);
    }

Esta funcion se encarga de hacer subir o bajar el monta-carga dependiendo de cual boton presione el usuario
ENTRADA_1 Y ENTRADA_2  #define que se utilizan para orientar el sentido de giro del motorl
dependiendo de cual boton presione el usuario el motor se mueve en un sentido o en otro(baja o sube) durante tres segundos(con delay),
el LED_VERDE indica que el monta-carga esta en movimiento, con las variables piso y acumulador se toma la referencia en que piso
esta para informarle al usuario



Link del proyecto
___________________________________________________________________________________________________________________
https://www.tinkercad.com/things/5Eu35WJHPGd-nahuel-gallardo1b-proyecto-domiciliario-para-parcial/editel?sharecode=7RycqCGOTAwI0Xi7EUitIe4qjQKl1Z5crGVPk3R_xsY

lenguaje  del programa
_________________________________________
C++
