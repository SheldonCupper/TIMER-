# Roteiro de testes do Louvor Pro

> Não usar o sistema em uma apresentação real sem testar previamente o equipamento, o navegador e a segunda tela.

## Segurança e conteúdo
- [ ] Adicionar aviso com título `<script>alert(1)</script>` e conferir que aparece como texto, sem executar JavaScript.
- [ ] Criar slide de músico com `<img src=x onerror=alert(1)>` e confirmar que a marcação é exibida literalmente.
- [ ] Testar texto bíblico retornado por fonte externa com caracteres `< > & "`.
- [ ] Conferir que nenhuma chave de API está disponível no código público.

## Apresentação e temporizador
- [ ] Criar, editar, selecionar e excluir avisos e slides.
- [ ] Abrir modo projetor em segunda janela/tela, verificar sincronização de texto e configurações.
- [ ] Testar cronômetro, pausa, reinício, aviso final e contagem até horário programado.
- [ ] Conferir blackout, modo retorno, tamanhos de texto e alinhamento.
- [ ] Testar bloqueador de popups e funcionamento em resoluções diferentes.

## Bíblia e armazenamento
- [ ] Consultar livros, capítulos e versículos com internet.
- [ ] Conferir mensagens quando uma API ou tradução estiver indisponível.
- [ ] Verificar opções de download e navegação offline sem presumir suporte a todas as traduções.
- [ ] Verificar persistência dos dados locais após recarregar a página.
- [ ] Conferir direitos/licenças de cada tradução antes de distribuir conteúdo.

## Limitações
O projeto é um protótipo web baseado no navegador. Testes de sintaxe não substituem testes manuais de interface e compatibilidade. Recursos bíblicos dependem de terceiros e podem falhar. Não coloque segredos de APIs dentro do `index.html`.
