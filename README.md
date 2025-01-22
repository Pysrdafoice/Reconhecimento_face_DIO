# Reconhecimento Facial com Nomeação Interativa

Este projeto realiza o reconhecimento de rostos em uma imagem e permite que o usuário nomeie cada rosto de forma interativa. Após a nomeação, o programa exibe a imagem original com os rostos enquadrados e identificados pelos nomes fornecidos.

## **Funcionalidades**
- Detecta rostos em uma imagem enviada pelo usuário.
- Permite recortar e exibir cada rosto detectado.
- Solicita ao usuário o nome para cada rosto.
- Salva os rostos recortados e nomeados em um diretório específico.
- Exibe a imagem original com os rostos enquadrados e identificados pelos nomes fornecidos.

---

## **Requisitos**
Certifique-se de ter as bibliotecas abaixo instaladas antes de executar o código:

- Python 3.7+
- face_recognition
- numpy
- opencv-python-headless
- Pillow

Instale as dependências necessárias com o seguinte comando:
```bash
pip install face_recognition numpy opencv-python-headless pillow
```

---

## **Como Usar**

### **1. Estrutura do Projeto**
Crie a seguinte estrutura de diretórios para o projeto:
```
project/
|— script.py            # Arquivo principal com o código
|— known_faces/         # Diretório onde os rostos nomeados serão salvos
```
O diretório `known_faces` será criado automaticamente se não existir.

### **2. Execute o Script**
Carregue o script em sua IDE ou ambiente Python e execute o arquivo `script.py`.

### **3. Envie uma Imagem**
Ao executar o script, será solicitado o upload de uma imagem contendo os rostos que você deseja identificar.
- Certifique-se de que a imagem está em formato suportado (JPEG ou PNG).

### **4. Nomeie os Rostos**
O programa detecta e exibe cada rosto individualmente. Para cada rosto:
- O rosto recortado é exibido.
- Você deve digitar o nome correspondente ao rosto ou pressionar **Enter** para marcá-lo como "Desconhecido".

### **5. Exibição Final**
Depois que todos os rostos forem nomeados:
- A imagem original é exibida com os rostos enquadrados e identificados pelos nomes fornecidos.
- Os rostos recortados são salvos no diretório `known_faces` com os nomes fornecidos.

---

## **Exemplo de Uso**
1. Execute o script:
   ```bash
   python script.py
   ```

2. Envie uma imagem com rostos.

3. O programa exibe os rostos detectados:
   - Digite o nome de cada rosto quando solicitado.
   - Exemplo:
     ```
     Rosto 1:
     Digite o nome para o rosto ou pressione Enter para "Desconhecido": Maria
     ```

4. Resultado Final:
   - A imagem original é exibida com os nomes sobre os rostos.
   - Os arquivos de rosto recortados são salvos no diretório `known_faces` com os nomes fornecidos.

---

## **Notas**
- Certifique-se de que a imagem enviada tenha boa iluminação e que os rostos sejam claramente visíveis.
- Se uma imagem contiver vários rostos muito próximos, a precisão da detecção pode variar.
- Este projeto usa o modelo `face_recognition`, que é baseado em deep learning para reconhecimento facial.

---

## **Melhorias Futuras**
- Adicionar suporte para upload de várias imagens.
- Implementar uma interface gráfica (GUI) para facilitar o uso.
- Melhorar o desempenho para imagens de alta resolução.

---

## **Licença**
Este projeto está sob a licença MIT. Sinta-se à vontade para usar, modificar e distribuir.


