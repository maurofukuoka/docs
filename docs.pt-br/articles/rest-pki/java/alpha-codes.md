﻿# Gerando códigos alfanuméricos em Java

[!include[Alpha Codes introduction](../../../includes/alpha-codes-intro.md)]

Você provavelmente copiou anteriormente os métodos (agora obsoletos) `generateVerificationCode`, `formatVerificationCode` e `parseVerificationCode`
dos exemplos para o seu código. Para atualizar a sua aplicação:

1. Atualize o pacote de nuget *com.lacunasoftware.restpki*
1. Substitua a implementação desses métodos no seu código por chamadas aos métodos da classe *AlphaCode*:

   ```java
   public static string generateVerificationCode() {
      return AlphaCode.generate();
   }
   
   public static string formatVerificationCode(String code) {
      return AlphaCode.format(code)
   }
   
   public static string parseVerificationCode(String formattedCode) {
      return AlphaCode.parse(formattedCode)
   }
   ```

[!include[Alpha Codes principles](../../../includes/alpha-codes-principles.md)]

## Veja também

* [Usando o Rest PKI em Java](index.md)