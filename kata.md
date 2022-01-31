
```bash
alias km='export E=katamarkon.txt'
alias kj='export E=katajoannen.txt'
alias kj2='export E=joannou2.txt'
alias r='enriched2model gr/$E out && enriched2latex gr/$E out && enriched2svg gr/$E out'
alias m='cat out/gr$(basename $E)'
alias x='(cd out; xelatex gr$(basename -s .txt $E).tex)'
alias e='(evince out/gr$(basename -s .txt $E).pdf)'
alias i='inkscape out/gr$(basename -s .txt $E).svg'
alias p='cp -vf out/*.png ~/img/kata/'
alias c='rm -rf out'
```
