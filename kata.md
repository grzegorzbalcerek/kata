
```bash
export E=katamarkon.txt
export E=katajoannen.txt
export E=joannou2.txt
alias p='enriched2model pl/$E out && enriched2latex pl/$E out && enriched2svg pl/$E out'
alias r='enriched2model $E out && enriched2latex $E out && enriched2svg $E out'
alias m='cat out/$(basename $E)'
alias t='cat out/$(basename -s .txt $E).tex'
alias x='(cd out; xelatex $(basename -s .txt $E).tex)'
alias e='(evince out/$(basename -s .txt $E).pdf)'
alias s='cat out/$(basename -s .txt $E).svg'
alias i='inkscape out/$(basename -s .txt $E).svg'
alias j='inkscape out/pl$(basename -s .txt pl/$E).svg'
alias c='rm -rf out'
```
