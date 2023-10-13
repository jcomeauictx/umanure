SERVER := $(notdir $(PWD))
DOCROOT := /var/www/$(SERVER)
DRYRUN ?= --dry-run
upload:
	rsync -avuz $(DRYRUN) $(DELETE) \
	 --exclude=Makefile \
	 . $(SERVER):$(DOCROOT)
