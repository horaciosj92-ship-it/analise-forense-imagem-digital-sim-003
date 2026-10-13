# Relatório Técnico Público — SIM-003

**Tipo:** síntese técnica anonimizada para portfólio.

## 1. Objetivo

Documentar os exames técnicos realizados em uma imagem JPEG, com foco em características estruturais, metadados e análises exploratórias de consistência visual. Este documento não substitui um laudo pericial completo.

## 2. Características do arquivo

- Formato: JPEG progressivo.
- Dimensões: 736 × 1600 pixels.
- Modo de cor: RGB.
- Subamostragem: YCbCr 4:2:0.
- Tamanho: 176.762 bytes.
- Validação estrutural com Pillow: concluída com sucesso.
- Validação pelo ExifTool: `Validate: OK`.
- Metadados EXIF de captura: não identificados nos exames registrados.
- Correspondência dos hashes entre a evidência recebida e a cópia de trabalho: confirmada nos registros do estudo.

A igualdade dos hashes indica correspondência binária entre os arquivos comparados no momento da verificação. Não comprova, isoladamente, a origem, a integridade histórica ou a veracidade do conteúdo visual.

## 3. Exames realizados no Forensically

### 3.1 JPEG Analysis

Foram examinadas características da estrutura JPEG, incluindo tabelas de quantização e codificação, além de marcadores associados ao formato progressivo.

O comportamento observado descreve características de codificação do arquivo. Isoladamente, essas características não permitem concluir que houve edição ou que a imagem permaneceu inalterada.

### 3.2 Error Level Analysis (ELA)

A análise foi realizada com diferentes configurações de qualidade JPEG, incluindo 90 e 95. Nas visualizações registradas, a distribuição residual foi descrita como relativamente uniforme, sem regiões isoladas claramente destacadas nas configurações utilizadas.

O resultado é exploratório. A aparência do mapa ELA depende de fatores como recompressão, conteúdo, resolução e parâmetros adotados. Não comprova nem exclui manipulação.

### 3.3 Noise Analysis

Foi utilizada amplitude de ruído 1, com equalização do histograma ativada e opacidade de visualização de 0,95.

A visualização foi descrita como apresentando distribuição aparentemente uniforme de granulação, sem discrepâncias localizadas claramente identificáveis na configuração utilizada.

Essa observação não demonstra que o ruído seja original da captura nem exclui alterações localizadas.

### 3.4 Level Sweep

Foi utilizada varredura de nível 1,00, largura 32 e opacidade de 0,95.

Foram observadas mudanças de exposição visual em diferentes áreas, incluindo elementos escuros e componentes da interface representada na imagem. O exame não permite determinar, por si só, a origem, o momento ou o método de criação desses elementos.

### 3.5 Luminance Gradient

A análise foi realizada com normalização ativada, equalização do histograma desativada, intensidade 2,00 e opacidade de 0,95.

A visualização apresentou variações de luminância associadas a elementos escuros e componentes da imagem. Não foi estabelecida, com esse exame isolado, uma causa específica para as variações observadas.

### 3.6 Clone Detection

A ferramenta foi utilizada com os parâmetros registrados durante o exame, incluindo bloco de tamanho 4 e tamanho máximo de imagem de 1024 pixels.

Foram observadas linhas coloridas sobre áreas com elementos repetitivos da interface. Esse resultado visual não basta para afirmar que houve clonagem ou duplicação deliberada de conteúdo. A interpretação exige considerar a disposição dos elementos, os parâmetros do detector e a possibilidade de correspondências naturais ou artefatos do método.

## 4. Síntese dos resultados

Os exames realizados caracterizam aspectos estruturais e visuais do arquivo. As observações obtidas com JPEG Analysis, ELA, Noise Analysis, Level Sweep, Luminance Gradient e Clone Detection não constituem, isoladamente, demonstração conclusiva de adulteração ou autenticidade.

A ausência de metadados EXIF de captura nos exames registrados não demonstra manipulação. Da mesma forma, uma validação estrutural bem-sucedida não comprova a origem ou a veracidade do conteúdo.

**Conclusão técnica: inconclusiva quanto à autenticidade integral ou à existência de manipulação da imagem**, considerando exclusivamente os exames documentados neste estudo.

## 5. Limitações

- Os resultados dependem das ferramentas, dos parâmetros e das condições de visualização utilizados.
- ELA, análise de ruído, varredura de níveis, gradiente de luminância e detecção de clones são exames exploratórios e não devem ser interpretados isoladamente.
- Não foi estabelecida, por esses exames, uma cadeia histórica completa de origem e custódia do arquivo.
- Não se afirma que a imagem seja autêntica ou falsa.
- A conclusão poderá ser reavaliada caso surjam arquivos de origem confiável, registros adicionais ou outros elementos técnicos pertinentes.

## 6. Próxima etapa recomendada

Caso esteja disponível, obter o arquivo original diretamente da fonte pertinente por procedimento documentado, registrar sua origem e calcular seu SHA-256. Comparar os arquivos preservando os originais e documentando eventuais diferenças binárias, estruturais e visuais.

## 7. Escopo da publicação

Esta publicação é uma síntese técnica anonimizada para fins de portfólio. A imagem examinada, o hash integral, os dados brutos e eventuais informações pessoais ou processuais permanecem fora do repositório público. Este documento não substitui um laudo pericial completo nem uma conclusão baseada em todos os elementos de um caso concreto.
