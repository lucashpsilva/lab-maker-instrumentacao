# 🔬 Laboratório Maker: Fabricação Digital para Instrumentação Científica

> **Do problema experimental ao instrumento físico.**

Este repositório nasceu a partir do minicurso **Laboratório Maker: Fabricação Digital para Instrumentação Científica**, apresentado na **XLIII Semana da Física da Universidade Federal de Goiás (UFG)** por **Lucas H. P. Silva**.

A proposta é transformar o conteúdo da apresentação em um **guia prático para estudantes, pesquisadores e profissionais que desejam desenvolver soluções de instrumentação dentro do laboratório**, utilizando fabricação digital, CAD, eletrônica, programação e ferramentas computacionais.

A premissa é simples:

> **A fabricação digital é uma ferramenta para transformar bits em átomos, mas o objetivo continua sendo responder à pergunta científica.**

---

## 🧭 Como utilizar este repositório

O conteúdo segue a mesma lógica apresentada no minicurso:

**Problema experimental**
↓
**Pesquisar antes de fabricar**
↓
**Projetar**
↓
**Simular quando necessário**
↓
**Fabricar**
↓
**Montar e testar**
↓
**Documentar e melhorar**

Você pode acompanhar a sequência completa ou consultar diretamente a etapa necessária para o seu projeto.

---

# 1. 🔬 O Problema — A Realidade dos Laboratórios

A instrumentação científica de alto nível pode envolver equipamentos de elevado custo, longos prazos de aquisição, dependência de importação e soluções altamente específicas.

Antes de pensar em fabricar uma solução, entretanto, a primeira pergunta deve ser:

> **O que o experimento realmente precisa?**

Nesta seção discutimos como identificar o problema, definir requisitos e avaliar quando uma solução comercial, uma adaptação ou uma fabricação própria faz sentido.

### 📖 Estudo de caso — Power Meter

Um dos exemplos apresentados no minicurso é o desenvolvimento de um **Power Meter de código aberto**, utilizado para discutir a possibilidade de desenvolver instrumentação científica de menor custo.

> 💡 **Ideia central:** o objetivo não é substituir indiscriminadamente equipamentos comerciais, mas avaliar tecnicamente quando uma solução aberta pode atender aos requisitos de uma determinada aplicação.

**Referência:** Santos et al. (2024)

**Veja também:**

* 🌎 [GOSH — Global Open Science Hardware](https://openhardware.science/)
* 📚 [Estudo de caso e referências](referencias/estudos_de_caso.md)

---

# 2. 🧠 A Mentalidade do Pesquisador-Maker

## Regra de ouro: não invente a roda

Fabricar não significa necessariamente fabricar tudo.

Um projeto de instrumentação pode combinar:

**componentes comerciais + peças fabricadas + eletrônica + software**

Por exemplo:

* motores;
* fusos;
* rolamentos;
* parafusos;
* perfis estruturais;
* sensores;
* componentes ópticos;
* microcontroladores;
* peças impressas em 3D.

A fabricação digital entra onde ela realmente agrega valor: **adaptação, personalização, prototipagem e fabricação de componentes específicos.**

### 🔎 Onde procurar?

#### Componentes e instrumentação

* 🔬 [Thorlabs](https://www.thorlabs.com/)
* ⚙️ [MISUMI](https://us.misumi-ec.com/)
* 🔩 [McMaster-Carr](https://www.mcmaster.com/)

#### Modelos CAD

* 📐 [GrabCAD](https://grabcad.com/library)
* 📐 [TraceParts](https://www.traceparts.com/)
* 📐 [3D ContentCentral](https://www.3dcontentcentral.com/)

> ⚠️ **Atenção:** encontrar um modelo CAD na internet não significa que ele possa ser utilizado livremente em qualquer projeto. Verifique a licença e as condições de uso antes de reutilizar ou redistribuir um modelo.

### 📋 Checklist

Antes de modelar uma peça do zero:

* [ ] O componente já existe comercialmente?
* [ ] O fabricante disponibiliza um modelo CAD?
* [ ] Existe uma alternativa compatível?
* [ ] Posso adaptar um componente existente?
* [ ] Fabricar a peça realmente reduz custo ou aumenta a funcionalidade?
* [ ] A solução atende aos requisitos do experimento?

---

# 3. 📐 Do Digital ao Físico

Esta é a etapa em que o problema experimental começa a se transformar em uma solução física.

Um fluxo típico é:

**Requisitos**

→ **CAD**

→ **Seleção de componentes**

→ **Simulação**

→ **Fabricação**

→ **Montagem**

→ **Teste**

→ **Iteração**

---

## 🔬 Estudo de caso — Z-Scan

O principal exemplo desenvolvido neste projeto é um **sistema de posicionamento linear motorizado de baixo custo para experimentos de óptica não linear (Z-Scan)**.

O projeto combina:

* modelagem CAD;
* componentes comerciais;
* peças fabricadas digitalmente;
* motores de passo;
* drivers;
* ESP32;
* firmware;
* controle de movimento;
* requisitos físicos do experimento.

### 📁 Arquivos do projeto

➡️ [Acessar o projeto Z-Scan](08_exemplos/z_scan/)

---

## 🧩 Projeto híbrido

Uma solução de instrumentação não precisa ser totalmente impressa.

No Z-Scan, por exemplo, componentes comerciais podem ser combinados com peças personalizadas fabricadas digitalmente.

Isso permite utilizar componentes disponíveis comercialmente onde eles são mais adequados e fabricar apenas aquilo que precisa ser personalizado.

---

# 4. 🤖 IA como ferramenta de desenvolvimento

Ferramentas de inteligência artificial podem ser utilizadas como **assistentes durante o desenvolvimento**, especialmente em tarefas como:

* programação;
* documentação;
* geração de código;
* análise de erros;
* exploração de alternativas;
* criação de modelos paramétricos;
* organização do projeto.

No projeto Z-Scan, a IA foi utilizada como auxílio no desenvolvimento do **firmware em C++ para ESP32**, a partir dos requisitos físicos e eletrônicos do sistema.

### ⚠️ Uma regra importante

A IA pode gerar código.

Ela não substitui:

* a análise física;
* a verificação elétrica;
* a validação experimental;
* a documentação;
* a responsabilidade do pesquisador.

O fluxo deve ser:

**Problema físico**

→ **Requisitos**

→ **Código gerado/auxiliado por IA**

→ **Revisão**

→ **Teste**

→ **Validação**

---

# 5. 🧮 Simulação e Gêmeos Digitais

Antes de fabricar uma peça, pode ser interessante verificar seu comportamento por meio de simulação.

Dependendo do problema, isso pode envolver:

* análise estrutural;
* elementos finitos (FEA);
* análise térmica;
* dinâmica;
* vibrações;
* outras técnicas de simulação.

### Fluxo

**CAD**

→ **Modelo para simulação**

→ **Malha**

→ **Condições de contorno**

→ **Simulação**

→ **Análise**

→ **Alteração do projeto**

→ **Fabricação**

A simulação é uma ferramenta de engenharia. **A validação experimental continua sendo necessária.**

### 🛠️ Ferramentas

* [Ansys](https://www.ansys.com/)
* [FreeCAD](https://www.freecad.org/)
* [Fusion](https://www.autodesk.com/products/fusion-360/overview)

---

# 6. 🖨️ Fabricando no Laboratório

Escolher o processo de fabricação é uma decisão de engenharia.

Não existe um processo universalmente melhor.

A escolha depende de fatores como:

* material;
* geometria;
* precisão;
* resistência;
* temperatura;
* ambiente químico;
* acabamento;
* custo;
* tempo de fabricação.

---

## 🧵 FDM

A fabricação por deposição de filamento pode ser utilizada para:

* suportes;
* adaptadores;
* carcaças;
* gabaritos;
* protótipos;
* componentes personalizados.

Materiais comuns incluem:

* PLA;
* PETG;
* ABS/ASA;
* outros polímeros específicos.

### Antes de imprimir

Considere:

* orientação da peça;
* altura de camada;
* número de paredes;
* preenchimento;
* suportes;
* temperatura;
* tolerâncias;
* anisotropia mecânica.

📁 [Guia de FDM](05_fabricacao/fdm.md)

---

# 7. 🧪 SLA / Impressão em Resina

A impressão em resina pode ser interessante quando o projeto exige:

* maior resolução;
* detalhes pequenos;
* geometrias complexas;
* superfícies mais suaves.

Entretanto, o material e o processo de pós-cura devem ser considerados durante o projeto.

Alguns aspectos importantes:

* propriedades mecânicas;
* fragilidade;
* estabilidade dimensional;
* compatibilidade química;
* exposição à luz;
* pós-processamento;
* segurança no manuseio.

📁 [Guia de SLA](05_fabricacao/sla.md)

> ⚠️ Parâmetros específicos de materiais, como formulações, misturas de resinas ou resistência química, devem ser tratados com referências experimentais ou dados do fabricante. Evite generalizar uma proporção ou propriedade para todas as resinas.

---

# 8. 📐 Projetar para Fabricar

Uma peça não deve ser projetada apenas para **existir no CAD**.

Ela precisa ser projetada considerando o processo que irá fabricá-la.

Isso inclui:

* orientação;
* suportes;
* tolerâncias;
* espessuras;
* interfaces;
* anisotropia;
* acabamento;
* montagem;
* manutenção.

---

## 🧭 Orientação da peça

Na impressão 3D, a orientação escolhida no fatiador influencia:

* quantidade de suportes;
* tempo de fabricação;
* acabamento;
* resistência mecânica;
* direção das camadas;
* comportamento da peça sob determinadas solicitações.

Por isso:

> **A orientação de fabricação faz parte do projeto mecânico.**

### Fatiadores

* [UltiMaker Cura](https://ultimaker.com/software/ultimaker-cura/)
* [PrusaSlicer](https://www.prusa3d.com/page/prusaslicer_424/)

📁 [Guia de projeto para FDM](05_fabricacao/fdm.md)

---

# 9. 📦 Documentação e Reprodutibilidade

Um projeto de laboratório não termina quando a peça sai da impressora.

Outra pessoa deve conseguir entender:

> **O que foi feito, por que foi feito e como reproduzir o resultado.**

Sempre que possível, registre:

* arquivos CAD;
* arquivos de fabricação;
* componentes utilizados;
* fornecedores;
* materiais;
* parâmetros;
* versões de software;
* código;
* problemas encontrados;
* alterações realizadas;
* resultados dos testes.

### Estrutura recomendada

```text
projeto/
├── CAD/
├── arquivos_3D/
├── eletronica/
├── firmware/
├── fabricacao/
├── documentacao/
├── imagens/
└── README.md
```

---

# 🔬 Projetos e exemplos

Os exemplos apresentados no minicurso serão organizados aqui como estudos de caso independentes.

| Projeto                       | Área               | Status                |
| ----------------------------- | ------------------ | --------------------- |
| [Z-Scan](08_exemplos/z_scan/) | Óptica / Automação | 🚧 Em desenvolvimento |
| Power Meter                   | Instrumentação     | 📖 Estudo de caso     |
| Outros projetos               | —                  | 🔜 Em construção      |

---

# 🔗 Recursos úteis

Uma lista mais completa de ferramentas, fabricantes, bibliotecas CAD, softwares e referências está disponível em:

👉 **[📚 Recursos e referências](referencias/recursos.md)**

---

# 📚 Referências

As referências utilizadas na apresentação e no desenvolvimento dos projetos estão organizadas em:

👉 **[📖 Referências](referencias/referencias.md)**

---

# 🤝 Contribuições

Este repositório pretende crescer além do minicurso.

Se você encontrar:

* uma ferramenta útil;
* uma biblioteca interessante;
* um fabricante;
* um modelo CAD;
* uma técnica de fabricação;
* uma referência;
* um erro neste material;

contribua por meio de uma **Issue** ou **Pull Request**.

A ideia é construir uma base de conhecimento aberta para quem utiliza fabricação digital como ferramenta de instrumentação científica.

---

# 👤 Autor

**Lucas H. P. Silva**

Engenharia Física — Universidade Federal de Goiás

📍 Goiânia, Brasil

---

> ### **Não se trata de imprimir tudo.**
>
> ### **Trata-se de saber quando, por que e como fabricar.**

