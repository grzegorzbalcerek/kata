
```bash
export E=katamarkon.txt
export E=katajoannen.txt
export E=joannou2.txt
alias r='enriched2model $E out/$(basename $E) && enriched2latex $E out/$(basename -s .txt $E).tex && enriched2svg $E out/$(basename -s .txt $E).svg'
alias m='cat out/$(basename $E)'
alias t='cat out/$(basename -s .txt $E).tex'
alias x='(cd out; xelatex $(basename -s .txt $E).tex)'
alias e='(evince out/$(basename -s .txt $E).pdf)'
alias s='cat out/$(basename -s .txt $E).svg'
alias i='inkscape out/$(basename -s .txt $E).svg'
alias c='rm -rf out'
```
