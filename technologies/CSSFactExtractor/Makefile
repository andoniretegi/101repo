# Comments are not supported.

test: 
	./extractor.py < test/Declaration.css > test/output/Declaration.json
	./extractor.py < test/Rule.css > test/output/Rule.json

	diff --ignore-all-space test/baseline/Declaration.json test/output/Declaration.json
	diff --ignore-all-space test/baseline/Rule.json test/output/Rule.json

	make reset-test
	
reset-test:
	@rm -f test/output/*.json

clean: 
	make reset-test

