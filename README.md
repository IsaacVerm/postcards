# Postcards

## Goal

Project according to best practices:

- documented
  - code
  - wiki
- tested
  - low level (unit or API tests)
  - E2E
- deployed early
- use virtual environment
- (optional) CLI

## Possible technologies

Either completely Django (Python):

- database included
- no separate API (so less modular)

Or flask (Python) with a Javascript framework (e.g. Elm):

- decoupled API
  - easier to plug other Javascript framework
  - can test with Postman
- more room for error

Since the project is still relatively vague at the moment a more Modular approach with flask is preferred.

E2E testing done with Cypress since it's very easy to use. API testing done with Postman.

If a CLI would be added Click is a popular Python library to do it.

## Example sites

Example sites and interesting functionality to reuse in own project.

- [postcardman.net](https://www.postcardman.net/)
  - show new postcards
  - quick view to glimpse at card
  - sort by dimension
- [teich](http://collections.carli.illinois.edu/cdm/landingpage/collection/nby_teich)
  - show cards on map
- [discogs](https://www.discogs.com)
  - explanations everywhere

What seems missing:

- filter on crucial criteria (e.g. has )

## Functionality

- add postcard
- update postcard
  - validation
- view postcards
  - filter
  - different types of views (e.g. with picture or not)
  - glimpse at postcard
  - analysis shows relation with other postcards

## Flask

Make app available: `export FLASK_APP=appname`

Activate debug mode: `export FLASK_ENV=development`

Run server: `flask run`

## API

Keep REST design principles in mind (e.g. [Programming historian](https://programminghistorian.org/en/lessons/creating-apis-with-python-and-flask#api-design-principles)).

## Testing

## Documentation

[Sphinx](http://www.sphinx-doc.org/) seems a good candidate since it's also used for the offical Python documentation.
