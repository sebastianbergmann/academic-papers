build :
		latexmk -pdf Thesis
		mv Thesis.pdf bergmann-WorkflowEngine-DiplomaThesis.pdf

clean :
		rm -f doxygen *.aux *.bak *.bbl *.blg *.lof *.log *.lot *.out *.pdf *.toc

dia :
		rm -f figures/grammar/*.pdf figures/architecture.pdf
		dia -e figures/grammar/axiom.eps -t eps-builtin figures/grammar/axiom.dia
		epstopdf figures/grammar/axiom.eps
		rm figures/grammar/axiom.eps
		dia -e figures/grammar/reduction.eps -t eps-builtin figures/grammar/reduction.dia
		epstopdf figures/grammar/reduction.eps
		rm figures/grammar/reduction.eps
		dia -e figures/grammar/and.eps -t eps-builtin figures/grammar/and.dia
		epstopdf figures/grammar/and.eps
		rm figures/grammar/and.eps
		dia -e figures/grammar/xor.eps -t eps-builtin figures/grammar/xor.dia
		epstopdf figures/grammar/xor.eps
		rm figures/grammar/xor.eps
		dia -e figures/grammar/or.eps -t eps-builtin figures/grammar/or.dia
		epstopdf figures/grammar/or.eps
		rm figures/grammar/or.eps
		dia -e figures/grammar/discriminator.eps -t eps-builtin figures/grammar/discriminator.dia
		epstopdf figures/grammar/discriminator.eps
		rm figures/grammar/discriminator.eps
		dia -e figures/architecture.eps -t eps-builtin figures/architecture.dia
		epstopdf figures/architecture.eps
		rm figures/architecture.eps

doxygen :
		rm -rf doxygen
		doxygen
		cp doxygen/latex/classezcWorkflowNode__inherit__graph.pdf figures/WorkflowNode.pdf
		cp doxygen/latex/classezcWorkflowNodeArithmeticBase__inherit__graph.pdf figures/WorkflowNodeArithmeticBase.pdf
		cp doxygen/latex/classezcWorkflowNodeBranch__inherit__graph.pdf figures/WorkflowNodeBranch.pdf
		cp doxygen/latex/classezcWorkflowNodeMerge__inherit__graph.pdf figures/WorkflowNodeMerge.pdf
		cp doxygen/latex/classezcWorkflowNodeSynchronization__inherit__graph.pdf figures/WorkflowNodeSynchronization.pdf
		cp doxygen/latex/classezcWorkflowNodeConditionalBranch__inherit__graph.pdf figures/WorkflowNodeConditionalBranch.pdf
		rm -rf doxygen
