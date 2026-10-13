# Relatório Técnico Público — SIM-003

**Tipo:** síntese técnica anonimizada para portfólio.

## 1. Objetivo

Documentar os exames técnicos realizados em uma imagem JPEG, com foco em suas características estruturais, metadados e análises exploratórias de consistência visual. Este documento não substitui um laudo pericial completo.

## 2. Características do arquivo

- **Formato:** JPEG progressivo.
- **Dimensões:** 736 × 1600 pixels.
- **Modo de cor:** RGB.
- **Subamostragem:** YCbCr 4:2:0.
- **Tamanho:** 176.762 bytes.
- **Validação estrutural com Pillow:** concluída com sucesso.
- **Validação pelo ExifTool:** `Validate: OK`.
- **Metadados EXIF de captura:** não identificados nos exames registrados.
- **Correspondência dos hashes:** os registros do estudo indicam igualdade entre o hash da evidência recebida e o da cópia de trabalho.

A igualdade dos hashes indica correspondência binária entre os arquivos comparados no momento da verificação. Não comprova, isoladamente, a origem, a integridade histórica ou a veracidade do conteúdo visual.

## 3. Exames realizados

### 3.1. Cálculo SHA-256

Foi calculado o hash SHA-256 da evidência recebida e da cópia de trabalho. Os registros disponíveis indicam valores iguais.

Esse resultado sustenta que os arquivos comparados eram binariamente correspondentes no momento da verificação. O hash, por si só, não demonstra quem criou a imagem, quando ela foi capturada ou se seu conteúdo já havia sido alterado antes do recebimento.

### 3.2. Extração de metadados com ExifTool

Foi utilizado o ExifTool para examinar as propriedades e os metadados disponíveis no arquivo.

Nos exames registrados, não foram identificados metadados EXIF de captura. Essa ausência não permite concluir que a imagem tenha sido manipulada, pois os metadados podem não estar presentes por diferentes motivos, inclusive pelo processo de criação, exportação ou compartilhamento do arquivo.

A validação estrutural informada pelo ExifTool retornou `Validate: OK`. Esse resultado se refere às verificações realizadas pela ferramenta e não certifica a autenticidade do conteúdo visual.

### 3.3. Validação estrutural com Pillow

Foi realizada a validação estrutural e a decodificação da imagem utilizando a biblioteca Pillow. O procedimento foi concluído com sucesso.

O resultado indica que o arquivo pôde ser processado pelo procedimento executado. Isso não comprova que a imagem corresponda a uma captura original ou que nunca tenha sido modificada.

### 3.4. JPEG Analysis

A ferramenta JPEG Analysis, do Forensically, foi utilizada para examinar características da estrutura JPEG, incluindo tabelas de quantização, tabelas de codificação e marcadores associados ao formato progressivo.

O exame permitiu observar características da codificação do arquivo. Essas características, isoladamente, não permitem concluir que houve edição nem demonstrar que a imagem permaneceu inalterada desde sua origem.

### 3.5. Error Level Analysis (ELA)

A análise ELA foi realizada com diferentes configurações de qualidade JPEG, incluindo 90 e 95. Nas visualizações registradas, a distribuição residual foi descrita como relativamente uniforme, sem regiões isoladas claramente destacadas nas configurações utilizadas.

A ELA é uma técnica exploratória cuja aparência pode variar conforme a recompressão, o conteúdo, a resolução e os parâmetros adotados. A distribuição visual dos resíduos não comprova nem exclui manipulação.

### 3.6. Noise Analysis

Foi utilizada amplitude de ruído 1, com equalização do histograma ativada e opacidade de visualização de 0,95.

A visualização foi descrita como apresentando distribuição aparentemente uniforme de granulação, sem discrepâncias localizadas claramente identificáveis na configuração utilizada.

Essa observação não demonstra que o ruído seja original da captura nem exclui alterações localizadas. A interpretação depende das características do arquivo e dos parâmetros da ferramenta.

### 3.7. Level Sweep

Foi utilizada varredura de nível 1,00, largura 32 e opacidade de 0,95.

Foram observadas mudanças na exposição visual de diferentes áreas, incluindo elementos escuros e componentes da interface representada na imagem.

O exame não permite determinar, por si só, a origem, o momento ou o método de criação desses elementos. As variações observadas devem ser interpretadas no contexto do conteúdo visual e das limitações da técnica.

### 3.8. Luminance Gradient

A análise foi realizada com normalização ativada, equalização do histograma desativada, intensidade 2,00 e opacidade de 0,95.

A visualização apresentou variações de luminância associadas a elementos escuros e componentes da imagem. Com base apenas nesse exame, não foi possível estabelecer uma causa específica para as variações observadas.

### 3.9. Clone Detection

A ferramenta Clone Detection foi utilizada com os parâmetros registrados durante o exame, incluindo bloco de tamanho 4 e tamanho máximo de imagem de 1024 pixels.

Foram observadas linhas coloridas sobre áreas que continham elementos repetitivos da interface.

Esse resultado visual não basta para afirmar que houve clonagem ou duplicação deliberada de conteúdo. A interpretação exige considerar a disposição dos elementos, os parâmetros do detector e a possibilidade de correspondências naturais ou artefatos produzidos pelo método.

## 4. Síntese dos resultados

Os exames realizados permitiram caracterizar aspectos estruturais e visuais do arquivo, bem como registrar observações produzidas por diferentes técnicas exploratórias.

As observações obtidas com JPEG Analysis, ELA, Noise Analysis, Level Sweep, Luminance Gradient e Clone Detection não constituem, isoladamente, demonstração conclusiva de adulteração ou autenticidade.

A ausência de metadados EXIF de captura nos exames registrados não demonstra manipulação. Da mesma forma, uma validação estrutural bem-sucedida não comprova a origem ou a veracidade do conteúdo.

**Conclusão técnica: inconclusiva quanto à autenticidade integral ou à existência de manipulação da imagem**, considerando exclusivamente os exames documentados neste estudo.

Essa conclusão não significa que a imagem seja autêntica ou adulterada, mas que os resultados registrados não permitem estabelecer uma conclusão definitiva sobre essas hipóteses.

## 5. Limitações

- Os resultados dependem das ferramentas, dos parâmetros e das condições de visualização utilizados.
- ELA, análise de ruído, varredura de níveis, gradiente de luminância e detecção de clones são exames exploratórios e não devem ser interpretados isoladamente.
- A validação estrutural não comprova a origem da imagem nem a integridade histórica de seu conteúdo.
- A ausência de metadados não demonstra, por si só, manipulação.
- A igualdade dos hashes comprova a correspondência binária entre os arquivos comparados no momento da verificação, mas não estabelece a procedência original da imagem.
- Não foi estabelecida, por esses exames, uma cadeia histórica completa de origem e custódia do arquivo.
- Não se afirma que a imagem seja autêntica ou falsa.
- A conclusão poderá ser reavaliada caso surjam arquivos de origem confiável, registros adicionais ou outros elementos técnicos pertinentes.

## 6. Próxima etapa recomendada

Caso esteja disponível, obter o arquivo original diretamente da fonte pertinente por meio de procedimento documentado, registrar sua origem e calcular seu hash SHA-256.

A comparação deverá preservar os arquivos originais e documentar eventuais diferenças binárias, estruturais e visuais, distinguindo observações técnicas de inferências.

## 7. Escopo da publicação

Esta publicação é uma síntese técnica anonimizada para fins de portfólio. A imagem examinada, o hash integral, os dados brutos e eventuais informações pessoais ou processuais permanecem fora do repositório público.

Este documento não substitui um laudo pericial completo nem uma conclusão baseada em todos os elementos de um caso concreto.
