# 🔬 Laboratório Maker: Fabricação Digital para Instrumentação Científica

Bem-vindo(a) ao repositório oficial do minicurso apresentado na **XLIII Semana da Física da UFG (2026)**! Aqui você encontra todos os arquivos, modelos 3D e códigos discutidos durante a apresentação.

## 🎯 Sobre o Projeto
Este repositório documenta a construção de um trasladador linear de baixo custo para a técnica de Z-scan, demonstrando como a integração entre peças comerciais, impressão 3D e microcontroladores pode democratizar o acesso à instrumentação científica de fronteira.

## 📂 Conteúdo do Repositório
*   **`/slides`**: Apresentação completa em formato PDF.
*   **`/cad_files`**: Arquivos `.STL` e `.STEP` do suporte do motor e porta-cubeta.
*   **`/firmware`**: Código fonte para ESP32 (controle do NEMA 17 via A4988).

## 🛠️ Lista de Materiais (BOM - Bill of Materials)
Para replicar o trasladador linear, você precisará de:
*   1x Microcontrolador ESP32
*   1x Motor de Passo NEMA 17
*   1x Driver de motor A4988
*   1x Fuso Trapezoidal T8 (Passo 2mm) com castanha
*   Peças impressas em 3D (PLA ou PETG)

## 🚀 Como Utilizar
1. Faça o download dos arquivos CAD na pasta correspondente.
2. Fatie os arquivos `.STL` utilizando a orientação sugerida (ver imagens na pasta).
3. Faça o upload do código `.ino` para o seu ESP32 via Arduino IDE.

---
*Desenvolvido por Lucas H. P. Silva*
