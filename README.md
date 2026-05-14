# Meu Mosquito AR

## Descrição
Esta atividade integra o **curso de imersão em realidade aumentada**, ministrado pelo iRede, e consiste em uma aplicação prática desenvolvida com os frameworks **A-Frame** e **AR.js**. O projeto utiliza um modelo 3D de mosquito chamado **Mosquito.glb**, com tamanho de **58,6 KB**, otimizado para execução em ambientes web.

A aplicação projeta o modelo sobre um marcador do tipo **Hiro** e foi ajustada para funcionar em dispositivos móveis e desktops com suporte a câmera. Nesta versão, a cena foi otimizada para reduzir o tempo até o primeiro aparecimento do modelo e melhorar o desempenho em aparelhos com menor capacidade gráfica.

## Configurações do Modelo
- **Posição**: `position="0 0 0"`
- **Escala**: `scale="1.5 1.5 1.5"`
- **Animação**: reprodução automática com `animation-mixer`

## Otimizações Aplicadas
- Pré-carregamento do modelo 3D com `a-assets`
- Indicador visual de carregamento durante a inicialização da câmera e do modelo
- Renderização configurada para priorizar desempenho em dispositivos móveis
- Redução da complexidade de iluminação para melhorar a performance

## Iluminação
A cena conta com:
- Uma luz ambiente para iluminação geral
- Uma luz direcional para destacar o modelo

## Renderização
A cena foi configurada com foco em desempenho, utilizando:
- `antialias` desativado
- `precision` configurado como `mediump`
- `powerPreference` ajustado para `high-performance`
- Correção de cores ativada

## Interações
1. **Pinch para zoom**: ajusta a escala do modelo com dois dedos.
2. **Rotação com um dedo**: permite rotacionar o modelo horizontal e verticalmente.
3. **Toque rápido**: dispara uma animação de pulso que aumenta e reduz a escala do modelo.

## Requisitos
- Navegador com permissão de câmera
- Dispositivo móvel ou desktop com câmera
- Boa iluminação no ambiente para facilitar a detecção do marcador Hiro
- Marcador Hiro visível e com contraste adequado

## Como executar
1. Acesse o link da aplicação.
Abra em seu navegador: **meumosquitoar.netlify.app**

2. Permita o uso da câmera.
Ao carregar a página, o navegador solicitará acesso à câmera. Clique em permitir para continuar.

3. Aguarde o carregamento inicial.
A aplicação exibe uma mensagem de carregamento enquanto inicializa a câmera e o modelo 3D.

4. Aponte para o marcador Hiro.
Com a câmera ativa, direcione-a para o marcador Hiro.
![Marcador Hiro](image.png)

## Tecnologias Utilizadas
- **A-Frame**: framework para desenvolvimento de experiências de realidade virtual e aumentada
- **AR.js**: biblioteca para AR baseada em marcadores
- **aframe-extras**: suporte à animação do modelo 3D
- **Modelo 3D**: `Mosquito.glb`