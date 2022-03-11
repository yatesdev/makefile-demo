# In a file with multiple targets, the first will be run by make without arguments
.PHONY: print
print:
	@echo "Hi this is a test"

.PHONY: world
world: hello
	@echo "world"

.PHONY: hello
hello:
	@echo "hello"

notPhony:
	@mkdir notPhony
