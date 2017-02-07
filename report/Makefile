SHELL=/bin/bash
NAME=report
INTRO=introduction
SEL=feature-selection
PCA=pca
PCA2=pca_data2
MANIFOLD=manifold-learning
MANIFOLD2=manifold-learning_data2
NN=neural-networks
NN2=neural-networks_data2

.PHONY: report, clean, introduction, feture_selection, pca, manifold_learning, neurlal_networks

report: ${INTRO}.pdf ${SEL}.pdf ${PCA}.pdf ${PCA2}.pdf ${MANIFOLD}.pdf ${MANIFOLD2}.pdf ${NN}.pdf ${NN2}.pdf
	pdftk ${INTRO}.pdf ${SEL}.pdf ${PCA}.pdf ${PCA2}.pdf ${MANIFOLD}.pdf ${MANIFOLD2}.pdf ${NN}.pdf ${NN2}.pdf cat output ${NAME}.pdf

clean:
	-rm ${NAME}.pdf
	-rm ${INTRO}.pdf
	-rm ${SEL}.pdf
	-rm ${PCA}.pdf
	-rm ${PCA2}.pdf
	-rm ${MANIFOLD}.pdf
	-rm ${MANIFOLD2}.pdf
	-rm ${NN}.pdf
	-rm ${NN2}.pdf

${INTRO}.pdf: ${INTRO}.tex
	pdflatex --shell-escape ${INTRO}.tex
	-rm ${INTRO}.{aux,log,nav,out,snm,toc}

${SEL}.pdf: ${SEL}.tex
	pdflatex --shell-escape ${SEL}.tex
	-rm ${SEL}.{aux,log,nav,out,snm,toc}

${PCA}.pdf: ${PCA}.tex
	pdflatex --shell-escape ${PCA}.tex
	-rm ${PCA}.{aux,log,nav,out,snm,toc}


${PCA2}.pdf: ${PCA2}.tex
	pdflatex --shell-escape ${PCA2}.tex
	-rm ${PCA2}.{aux,log,nav,out,snm,toc}


${MANIFOLD}.pdf: ${MANIFOLD}.tex
	pdflatex --shell-escape ${MANIFOLD}.tex
	-rm ${MANIFOLD}.{aux,log,nav,out,snm,toc}


${MANIFOLD2}.pdf: ${MANIFOLD2}.tex
	pdflatex --shell-escape ${MANIFOLD2}.tex
	-rm ${MANIFOLD2}.{aux,log,nav,out,snm,toc}


${NN}.pdf: ${NN}.tex
	pdflatex --shell-escape ${NN}.tex
	-rm ${NN}.{aux,log,nav,out,snm,toc}


${NN2}.pdf: ${NN2}.tex
	pdflatex --shell-escape ${NN2}.tex
	-rm ${NN2}.{aux,log,nav,out,snm,toc}

