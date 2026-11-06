# DigitaHinos FingerStyle

Hinos no violão folk com cutaway (preto, com detalhes bege) com **partitura e tablatura dinâmicas**.

- Tela única: botões **Hinos**, **Instalar** (aplicativo) e **Pix**.
- Menu **Tela**: violão + partitura, só o violão ou só a partitura/tablatura.
- Botão **⬇ PDF**: baixa a partitura/tablatura do hino (segue o formato escolhido no menu Partitura).
- Menu **Partitura**: notação + tablatura, ou só tablatura (com o nome e o diagrama de cada acorde acima da tablatura). A partitura aparece numa moldura 16:9 com 2 a 3 linhas por vez e vira a "página" sozinha.
- Mão esquerda animada (com limite de alcance realista, dedos numerados, que pode ser ocultada em Opções → Mão); sem notinhas subindo.
- Sem tela de edição e sem modo Acompanhamento.
- **Modo Pro** (`pro-config.js` + `apps-script/`): código de uso único por aparelho, validado numa planilha Google. No modo grátis tudo é liberado (todos os hinos, velocidade, PDF, partitura dinâmica); só a **escolha de tom** é Pro. Para voltar a limitar hinos, ajuste `freeHinos`/`previewSec` em `pro-config.js`.

## Publicação
Suba os arquivos no GitHub Pages. A cada versão nova, mude `CACHE_NAME` em `sw.js`.
O workflow `.github/workflows/build-apk.yml` gera o APK (Capacitor).

## Adornos
No soprano o app coloca, em poucos pontos bem escolhidos e fáceis de tocar: ligado (H), puxada (P), slide (sl.) e vibrato (onda). Aparecem na tablatura/PDF e no som (o ligado e a puxada mudam a altura da nota que já soa, o slide desliza entre as casas e o vibrato oscila a altura); podem ser desligados em ⚙ Opções → Adornos.

## Harmonia Cantoral (livro)
O arquivo `hinos/cifras.json` traz as cifras do Hinário 5 (CCB) já alinhadas a compasso e tempo de cada hino; o app transpõe sozinho para o tom escolhido. Hinos que não estão no arquivo usam a harmonia Simples quando se escolhe "Cantoral". Lista dos hinos sem cifra: `hinos/SEM-CIFRA.txt`.
