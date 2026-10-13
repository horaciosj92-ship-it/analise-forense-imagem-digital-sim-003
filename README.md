# Análise Forense de Imagem Digital — SIM-003

## Objetivo
Estudo técnico de análise de imagem JPEG com foco em integridade,
metadados e validação estrutural.

## Ferramentas
- Python
- ExifTool 12.76
- Pillow
- SHA-256
- Análise exploratória Error Level Analysis (ELA)

## Resultados técnicos
- Formato: JPEG progressivo
- Dimensões: 736 × 1600 pixels
- Modo de cor: RGB
- Subamostragem: YCbCr 4:2:0
- Tamanho analisado: 176.762 bytes
- Validação estrutural com Pillow: concluída com sucesso
- ExifTool: Validate OK
- Metadados EXIF de captura: não identificados nos exames registrados
- Perfil ICC e comentário JPEG: não identificados pelo Pillow
- Hash da evidência e da cópia de trabalho: iguais

## Conclusão
Os exames realizados não permitem confirmar nem excluir a autenticidade
integral ou a manipulação da imagem. A igualdade dos hashes demonstra
a correspondência binária entre a evidência recebida e a cópia de trabalho,
não a origem ou a veracidade do conteúdo visual.

A análise ELA é exploratória e não constitui prova isolada de edição.

## Limitações
Este material público é uma síntese técnica anonimizada. Não contém a
imagem examinada, identificadores processuais, hash integral ou registros
brutos. Não substitui um laudo completo nem uma comparação com o arquivo
original obtido de fonte oficial.

## Reprodutibilidade
Os resultados aqui descritos correspondem aos exames registrados no
estudo de caso. Não se afirma que os testes provem a autenticidade
ou a falsidade da imagem.
