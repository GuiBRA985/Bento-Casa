# Casa Bento — Chez Rose, Pousada VIP

A Chez Rose oferece a expedição Chapada dos Guimarães em seu mapa personalizado. Base de todos os passeios: **-15.470382, -55.749426**. Traslado: Aeroporto Marechal Rondon, Várzea Grande → Chez Rose.

## Atualizar o mapa

Edite `mapas/chez-rose.json`: dados da pousada, telefone de orçamento, aeroporto e lista `expedicoes`. Cada expedição contém suas próprias `atracoes` (id, nome, descrição, latitude e longitude). O seletor apresenta todas as expedições desse arquivo. A página aponta para ele pelo atributo `data-map-source` em `index.html`; outro cliente VIP pode ter seu próprio arquivo.

Não coloque senhas nem informações privadas nesse arquivo público. O arquivo é o catálogo publicado; não exige banco de dados. Esta versão não inclui painel administrativo nem sincronização do aplicativo Android.

## Funcionamento

- Atrações: marcadores, seleção de passeios e navegação com saída e retorno à Chez Rose.
- Traslado: aeroporto e pousada no mapa; rota rodoviária no Google Maps.
- Orçamento: nome, chegada prevista, pessoas, dias, atrações e pedido de traslado; abre WhatsApp para o visitante enviar à pousada.
- As rotas são calculadas no Google Maps, sem desenhar linhas retas como se fossem estradas. O link conjunto apresenta até nove atrações; cada atração também tem seu link próprio. O pedido de orçamento inclui todas as escolhidas.
- Fotos, hospedagem via Airbnb e localização existentes foram preservadas.
- Interface do mapa em português, inglês, espanhol e francês. Nomes e descrições do catálogo são cadastrados em português.

Publicação via GitHub Pages usando `main`, com o domínio existente em `CNAME`. O mapa depende de Leaflet e dos mapas OpenStreetMap online. Disponibilidade de passeios, acessos, guias e valores é confirmada pela pousada.
