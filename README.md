# 📱 CryptoMonitor

**Checkpoint 2 – Android Kotlin Developer**  
**Aluno:** Rafael Villela – **RM:** 550275  

🔗 Baseado no projeto do professor [Ewerton Luiz de Lima Carreira](https://github.com/carreiras/android-crypto-monitor)

---

## 🎯 Sobre o Projeto

O aplicativo **CryptoMonitor** foi desenvolvido para consultar e exibir o **último valor de cotação do Bitcoin (BTC)**, utilizando a API pública do **Mercado Bitcoin**.

Com o botão **Refresh**, o usuário atualiza manualmente a cotação, visualizando:

- 📈 O último preço do Bitcoin;
- 🕒 A data e hora da última atualização.

---

## 📱 Resultado Final

<p align="center">
  <img src="![image](https://github.com/user-attachments/assets/c800fadf-c2c7-4789-b58d-7e7259650e16)" alt="Tela do Aplicativo CryptoMonitor" />
</p>

---

## 🧩 Evidências do Código

### 1. Modelagem dos dados (`TickerResponse.kt`)

<p align="center">
  <img src="![image](https://github.com/user-attachments/assets/465ab3af-45b3-41c5-9c47-da79b0b69231)" alt="Código - TickerResponse" />
</p>

Criação da estrutura de dados para representar a resposta da API.

---

### 2. Interface de comunicação (`MercadoBitcoinService.kt`)

<p align="center">
  <img src="![image](https://github.com/user-attachments/assets/610f63df-a689-4028-8756-9aec9267b529)" alt="Código - MercadoBitcoinService" />
</p>

Definição do método HTTP GET para buscar o ticker do Bitcoin.

---

### 3. Fábrica de Serviço (`MercadoBitcoinServiceFactory.kt`)

<p align="center">
  <img src="![image](https://github.com/user-attachments/assets/941badaf-6abd-4be9-b388-d15ce1529d4a)" alt="Código - MercadoBitcoinServiceFactory" />
</p>

Criação e configuração do Retrofit para chamadas de rede.

---

### 4. Configuração Inicial (`MainActivity.kt` - Parte 1)

<p align="center">
  <img src="![image](https://github.com/user-attachments/assets/75e9c1f9-b6b5-4f55-aac3-d4ab37e15da7)" alt="Código - MainActivity Parte 1" />
</p>

Inicialização da Toolbar e do botão Refresh.

---

### 5. Chamada da API e atualização da UI (`MainActivity.kt` - Parte 2)

<p align="center">
  <img src="![image](https://github.com/user-attachments/assets/e5791949-1b60-45cb-9a0b-0c8848c7b729)" alt="Código - MainActivity Parte 2" />
</p>

Execução da chamada assíncrona para obter dados da API e atualização dos elementos visuais.

---

## 🔎 Explicação Geral do Funcionamento

- **Retrofit**: utilizado para fazer a chamada à API de forma simples e segura.
- **Coroutines**: permitem realizar a comunicação de rede sem bloquear a interface do usuário.
- **Formatação**: os dados recebidos são formatados para o padrão brasileiro (moeda e data).
- **Tratamento de erros**: mensagens de erro são exibidas usando Toasts para melhorar a experiência do usuário.

---

## ✅ Conclusão

O projeto permitiu praticar:

- Comunicação com APIs REST em Kotlin;
- Utilização de Retrofit e Coroutines em projetos Android;
- Boas práticas de formatação e exibição de dados;
- Organização de código seguindo padrões de projeto.

---

# 🚀 Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/carreiras/android-crypto-monitor
   ```
2. Abra o projeto no Android Studio.
3. Execute em um dispositivo ou emulador Android.

---

**Desenvolvido por:** Rafael Villela – RM: 550275
