# articles-annotations

## Etapas para transformar o caminho absoluto em relativo do pdf no *file system*:

1) Suponha o artigo.pdf. Ele é salvo pela interface do *xournal* como *arquivo.pdf.xoj*, primeiramento renomeamos arquivo para ter a extensão *.gz*:

    mv arquivo.pdf.xoj arquivo.pdf.xoj.gz

2) Descompactamos o *arquivo.pdf.xoj.gz*:

    gunzip arquivo.pdf.xoj.gz
    
3) Editamos o xoj:

    vim arquivo.pdf.xoj

4) Compactamos o arquivo alterado:

    gzip arquivo.pdf.xoj
 
 5) Voltamos ele para a extensão original:
 
     mv arquivo.pdf.xoj.gz arquivo.pdf.xoj
 
