# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Bacon-Goodman decomposition for differences-in-differences estimation with variation in treatment timing Use bacondecomp With (In) R Software
# Decomposition for differences-in-differences estimation with variation in treatment timing from Goodman-Bacon (2018) Use bacondecomp With (In) R Software
install.packages("bacondecomp")
install.packages("ggplot2")
library("bacondecomp")
library("ggplot2")
bacondecomp = read.csv("https://raw.githubusercontent.com/timbulwidodostp/bacondecomp_r/main/bacondecomp/bacondecomp.csv",sep = ";")
# Estimation
# Bacon-Goodman decomposition for differences-in-differences estimation with variation in treatment timing Use bacondecomp With (In) R Software
# Decomposition for differences-in-differences estimation with variation in treatment timing from Goodman-Bacon (2018) Use bacondecomp With (In) R Software
bacondecomp <- bacon(incearn_ln ~ reform_math, data = bacondecomp, id_var = "state", time_var = "class")
ggplot(bacondecomp) +
aes(x = weight, y = estimate, shape = factor(type)) +
geom_point() +
geom_hline(yintercept = 0) +
labs(x = "Weight", y = "Estimate", shape = "Type")
# Bacon-Goodman decomposition for differences-in-differences estimation with variation in treatment timing Use bacondecomp With (In) R Software
# Decomposition for differences-in-differences estimation with variation in treatment timing from Goodman-Bacon (2018) Use bacondecomp With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished