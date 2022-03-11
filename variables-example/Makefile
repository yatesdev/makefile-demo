FIRST_NAME := Steve # defined immediately
NOT_FULL_NAME := ${FIRST_NAME} ${LASTNAME}
FULL_NAME = ${FIRST_NAME} ${LASTNAME} # Lazily defined
LASTNAME = Jobs

files = other-name.txt not-full-name.txt full-name.txt

all: $(files)

other-name.txt: LASTNAME = Irwin
other-name.txt:
	@echo "${FULL_NAME}" > other-name.txt

not-full-name.txt:
	@echo "${NOT_FULL_NAME}" > not-full-name.txt

full-name.txt:
	@echo "${FULL_NAME}" > full-name.txt

.PHONY: clean
clean:
	@rm other-name.txt
	@rm not-full-name.txt
	@rm full-name.txt