
```bash
alias km='export E=katamarkon.txt'
alias kj='export E=katajoannen.txt'
alias kj2='export E=joannou2.txt'
alias r='enriched2model gr/$E out && enriched2latex gr/$E out && enriched2svg gr/$E out && enriched2model pl/$E out && enriched2latex pl/$E out && enriched2svg pl/$E out'
alias mg='cat out/gr$(basename $E)'
alias mp='cat out/pl$(basename $E)'
alias xg='(cd out; xelatex gr$(basename -s .txt $E).tex)'
alias xp='(cd out; xelatex pl$(basename -s .txt $E).tex)'
alias eg='(evince out/gr$(basename -s .txt $E).pdf)'
alias ep='(evince out/pl$(basename -s .txt $E).pdf)'
alias ig='inkscape out/gr$(basename -s .txt $E).svg'
alias ip='inkscape out/pl$(basename -s .txt pl/$E).svg'
alias c='rm -rf out'
```
