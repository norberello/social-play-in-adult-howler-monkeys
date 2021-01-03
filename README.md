# Social play in adult howler monkeys
<center>
    <img src="figures/two adult males and one adult female playing.png" width="50%" alt="" class="center" align="middle" alt="howler adult monkeys playing">
</center>
<p>
R scripts and databases used to study social play in adult howler monkeys for the study 'Socioecological correlates of social play in adult howler monkeys (<i>Alouatta palliata mexicana<i/> and <i>A. p. palliata<i/>)'
<p>  
    
```
#par(mar = c(bottom, left, top, right)) 
#two plots together
par(mar=c(5,4.5,2,1),cex.lab=2)
par(mfrow=c(1,2))
boxplot(data.ptime$X.PLAYTOTAL ~ data.ptime$CLASS ,
                   ylab="% social play" ,
                   xlab="age class",outline=FALSE,main=
                     "a",cex.lab=1.5,medcol="red",
        varwidth = TRUE,
        col = "lightgray")
points(c(1.4,2.16,0.84,0.61),pch=3,cex=1.5)
plot(data.playage$MONTHS,data.playage$PLAY.P,
     pch = 16,
     col="blue",xlab = "age (months)",cex=0.76, 
     ylab = "% social play",main="b",cex.lab=1.5)
lines(newdata.months$MONTHS, predicted.months$fit*100,lwd=2,col=2)
lines(newdata.months$MONTHS, predicted.months$fit*100+
        predicted.months.int*100,lty=3)
lines(newdata.months$MONTHS, predicted.months$fit*100-
        predicted.months.int*100,lty=3)
```

<img src="figures/fig1.png" alt="Simply Easy Learning">
<p>
<b>Figure 1.</b> (a) Changes in social play in howler monkeys according to age class (I: immatures, J: Juveniles, SA: subadults, A: adults). Solid lines and crosses within the box marks the median and mean, respectively. The boundary of the box closest to 0 indicates the 25th percentile (first quartile), and the boundary of the box farthest from zero indicates the 75th percentile (fourth quartile). The whiskers denote the minimum and maximum values. (b) Relationship between age (months) and social play; 95% confidence intervals are shown in grey dotted lines around the solid regression line.
    
   
