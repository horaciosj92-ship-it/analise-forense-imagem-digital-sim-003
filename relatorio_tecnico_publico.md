# Relatório Técnico Público — SIM-003

**Tipo:** síntese técnica anonimizada para portfólio.

## 1. Objetivo

Documentar os exames técnicos realizados em uma imagem JPEG, com foco nas características estruturais do arquivo, nos metadados disponíveis e nas análises exploratórias de consistência visual. Este documento apresenta os procedimentos e as observações registrados no estudo, sem substituir um laudo pericial completo.

## 2. Características do arquivo

- **Formato:** JPEG progressivo.
- **Dimensões:** 736 × 1600 pixels.
- **Modo de cor:** RGB.
- **Subamostragem de crominância:** YCbCr 4:2:0.
- **Tamanho:** 176.762 bytes.
- **Validação estrutural com Pillow:** concluída com sucesso.
- **Validação pelo ExifTool:** resultado registrado como `Validate: OK`.
- **Metadados EXIF de captura:** não identificados nos exames registrados.
- **Correspondência dos hashes:** os registros do estudo indicam igualdade entre os hashes da evidência recebida e da respectiva cópia de trabalho.

A igualdade dos hashes indica correspondência binária entre os arquivos comparados no momento da verificação. Isoladamente, não comprova a origem da imagem, sua integridade histórica nem a veracidade de seu conteúdo visual.

## 3. Exames realizados

### 3.1. Cálculo do hash SHA-256

Foi calculado o hash SHA-256 da evidência recebida e da cópia de trabalho. Os registros disponíveis indicam que os valores obtidos foram iguais.

Esse resultado sustenta que os arquivos comparados eram binariamente idênticos no momento da verificação. O hash, por si só, não identifica quem criou a imagem, quando ocorreu a captura nem se o conteúdo já havia sido alterado antes do recebimento.

### 3.2. Extração de metadados com ExifTool

O ExifTool foi utilizado para examinar as propriedades e os metadados disponíveis no arquivo.

Nos exames registrados, não foram identificados metadados EXIF de captura. Essa ausência não permite concluir que a imagem tenha sido manipulada, pois os metadados podem estar ausentes por diferentes motivos, inclusive em decorrência do processo de criação, exportação ou compartilhamento do arquivo.

A validação informada pelo ExifTool retornou `Validate: OK`. Esse resultado deve ser interpretado no âmbito das verificações realizadas pela ferramenta e não certifica a autenticidade do conteúdo visual.

### 3.3. Validação estrutural com Pillow

Foi realizada a validação estrutural e a decodificação da imagem utilizando a biblioteca Pillow. O procedimento foi concluído com sucesso.

Esse resultado indica que o arquivo pôde ser processado pelo procedimento executado. Não comprova que a imagem corresponda a uma captura original nem que seu conteúdo nunca tenha sido modificado.

### 3.4. Análise da estrutura JPEG

A ferramenta JPEG Analysis, do Forensically, foi utilizada para examinar características da estrutura JPEG, incluindo tabelas de quantização, tabelas de codificação e marcadores associados ao formato progressivo.

O exame permitiu observar características da codificação do arquivo. Essas características, isoladamente, não permitem concluir que houve edição nem demonstrar que a imagem permaneceu inalterada desde sua origem.

### 3.5. Análise do Nível de Erro (ELA)

A análise ELA (*Error Level Analysis*) foi realizada com diferentes configurações de qualidade JPEG, incluindo 90 e 95. Nas visualizações registradas, a distribuição dos resíduos foi descrita como relativamente uniforme, sem regiões isoladas claramente destacadas nas configurações utilizadas.

A ELA é uma técnica exploratória cuja aparência pode variar conforme a recompressão, o conteúdo da imagem, a resolução e os parâmetros adotados. A distribuição visual dos resíduos não comprova nem exclui a existência de manipulação.

### 3.6. Análise de ruído

Foi utilizada amplitude de ruído 1, com equalização do histograma ativada e opacidade de visualização de 0,95.

A visualização foi descrita como apresentando distribuição aparentemente uniforme de granulação, sem discrepâncias localizadas claramente identificáveis na configuração utilizada.

Essa observação não demonstra que o ruído seja originário da captura nem exclui alterações localizadas. A interpretação depende das características do arquivo, do conteúdo analisado e dos parâmetros da ferramenta.

### 3.7. Varredura de nível

Foi utilizada a ferramenta Level Sweep com nível 1,00, largura 32 e opacidade de 0,95.

Foram observadas mudanças na exposição visual de diferentes áreas, incluindo elementos escuros e componentes da interface representada na imagem.

O exame não permite determinar, por si só, a origem, o momento ou o método de criação desses elementos. As variações observadas devem ser interpretadas considerando o conteúdo visual e as limitações da técnica.

### 3.8. Gradiente de luminância

A análise Luminance Gradient foi realizada com normalização ativada, equalização do histograma desativada, intensidade 2,00 e opacidade de 0,95.

A visualização apresentou variações de luminância associadas a elementos escuros e componentes da imagem. Com base apenas nesse exame, não foi possível estabelecer uma causa específica para as variações observadas.

### 3.9. Detecção de clones

A ferramenta Clone Detection foi utilizada com os parâmetros registrados durante o exame, incluindo tamanho de bloco 4 e tamanho máximo de imagem de 1024 pixels.

Foram observadas linhas coloridas sobre áreas que continham elementos repetitivos da interface.

Esse resultado visual não basta para afirmar que houve clonagem ou duplicação deliberada de conteúdo. A interpretação exige considerar a disposição dos elementos, os parâmetros do detector e a possibilidade de correspondências naturais ou artefatos produzidos pelo método.

## 4. Síntese dos resultados

Os exames realizados permitiram caracterizar aspectos estruturais e visuais do arquivo, além de registrar as observações produzidas por diferentes técnicas exploratórias.

As observações obtidas com JPEG Analysis, ELA, Noise Analysis, Level Sweep, Luminance Gradient e Clone Detection não constituem, isoladamente, demonstração conclusiva de adulteração ou de autenticidade.

A ausência de metadados EXIF de captura nos exames registrados não demonstra manipulação. Da mesma forma, uma validação estrutural bem-sucedida não comprova a origem nem a veracidade do conteúdo visual.

**Conclusão técnica: inconclusiva quanto à autenticidade integral ou à existência de manipulação da imagem**, considerando exclusivamente os exames documentados neste estudo.

Essa conclusão não significa que a imagem seja autêntica ou adulterada. Significa que os resultados registrados, considerados isoladamente e em conjunto, não permitem estabelecer uma conclusão definitiva sobre essas hipóteses.

## 5. Limitações

- Os resultados dependem das ferramentas, dos parâmetros e das condições de visualização utilizados.
- ELA, análise de ruído, varredura de nível, gradiente de luminância e detecção de clones são técnicas exploratórias e não devem ser interpretadas isoladamente.
- A validação estrutural não comprova a origem da imagem nem a integridade histórica de seu conteúdo.
- A ausência de metadados não demonstra, por si só, manipulação.
- A igualdade dos hashes comprova a correspondência binária entre os arquivos comparados no momento da verificação, mas não estabelece a procedência original da imagem.
- Os exames documentados não estabeleceram uma cadeia histórica completa de origem e custódia do arquivo.
- Não se afirma que a imagem seja autêntica ou falsa.
- A conclusão poderá ser reavaliada caso sejam disponibilizados arquivos de origem confiável, registros adicionais ou outros elementos técnicos pertinentes.

## 6. Próxima etapa recomendada

Caso esteja disponível, recomenda-se obter o arquivo original diretamente da fonte pertinente, por meio de um procedimento documentado de coleta. A origem deverá ser registrada, e o hash SHA-256 deverá ser calculado e documentado.

A comparação deve preservar os arquivos originais e registrar eventuais diferenças binárias, estruturais e visuais, distinguindo observações técnicas de inferências.

## 7. Escopo da publicação

Esta publicação é uma síntese técnica anonimizada para fins de portfólio. A imagem examinada, o hash integral, os dados brutos e eventuais informações pessoais ou processuais permanecem fora do repositório público.

Este documento não substitui um laudo pericial completo nem uma conclusão fundamentada em todos os elementos de um caso concreto.
