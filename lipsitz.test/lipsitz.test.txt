# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Lipsitz goodness of fit test for ordinal logistic models Use lipsitz.test (generalhoslem) With (In) R Software
install.packages("generalhoslem")
install.packages("ordinal")
library("generalhoslem")
library("ordinal")
lipsitz.test = read.csv("https://raw.githubusercontent.com/timbulwidodostp/lipsitz.test/main/lipsitz.test/lipsitz.test.csv",sep = ";")
# Estimation Lipsitz goodness of fit test for ordinal logistic models Use lipsitz.test (generalhoslem) With (In) R Software
lipsitz.test$gear <- as.factor(lipsitz.test$gear)
polr <- polr(gear ~ mpg + cyl, data = lipsitz.test)
lipsitz.test(polr)
clm <- clm(gear ~ mpg, data = lipsitz.test)
lipsitz.test(clm)
# Lipsitz goodness of fit test for ordinal logistic models Use lipsitz.test (generalhoslem) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
