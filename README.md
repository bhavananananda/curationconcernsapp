# CurationConcerns
# https://github.com/samvera/curation_concerns

This is a rails application that uses curation_concerns gem adding the ability to
Create, Read, Update and Destroy (CRUD) objects (based on Hydra::Works) 

# Note
This gem depends on hydra-works/fedora/solr/db

# Get the solr running at http://localhost:8983/solr
```bash
When running for the first time:
solr_wrapper -p 8984 -d solr/config/ --collection_name hydra-curationconcerns

When running for successive times:
solr_wrapper &
```

# Get the fedora running at http://localhost:8984/rest
```bash
To specify a different port:
fcrepo_wrapper -p 8984 --no-jms

Or just run:
fcrepo_wrapper &
```

# Get this app working on http://localhost:3000

```bash
Clone this app
bundle install
rake assets:precompile
rails server -b 0.0.0.0 
```
Access the application at http://localhost:3000

Bingo!

