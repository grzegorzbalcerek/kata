
```bash
export E=katamarkon.txt
export E=katajoannen.txt
export E=joannou2.txt
alias p='enriched2model pl/$E out/pl/$(basename pl/$E) && enriched2latex $E out/pl/$(basename -s .txt pl/$E).tex && enriched2svg pl/$E out/pl/$(basename -s .txt pl/$E).svg'
alias r='enriched2model $E out/$(basename $E) && enriched2latex $E out/$(basename -s .txt $E).tex && enriched2svg $E out/$(basename -s .txt $E).svg'
alias m='cat out/$(basename $E)'
alias t='cat out/$(basename -s .txt $E).tex'
alias x='(cd out; xelatex $(basename -s .txt $E).tex)'
alias e='(evince out/$(basename -s .txt $E).pdf)'
alias s='cat out/$(basename -s .txt $E).svg'
alias i='inkscape out/$(basename -s .txt $E).svg'
alias j='inkscape out/pl/$(basename -s .txt pl/$E).svg'
alias c='rm -rf out'
```
