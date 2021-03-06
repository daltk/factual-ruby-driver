## v1.3.4
* multi requests as POST

## v1.3.3
* fixed bug in multi #12

## v1.3.2
* added integration test for unicode queries
* added insert
* changed factual-auth yaml file from under the integration test folder to ~/.factual
* added clear
* timeout support

## v1.3.1
* removed sugar crosswalk, switch to normal table

## v1.3
* added diffs
* changed raw read to get 
* added raw post
* moved README to wiki
* added match

## v1.2.1
* crosswalk endpoint change

## v1.2
* releasing geo features, facets, writes, multi and monetize

## v1.1.9
* added geocode, geopulse and world-geographies
* added facets
* adding writes (submit, flag)
* updated documents
* added multi
* added monetize

## v1.1
* added debug mode
* added raw read

## v1.0.3
* added crosswalk(namespace_id, namespace)

## v1.0.2
* lazy getting total_count of a query
* changed Query#total_rows to Query#total_count to be consistent

## v1.0.1
* fixed url escape for .filters(:category => "Food & Beverage > Restaurants")

## v1.0.0
* fully documented
* crosswalk(<factual_id>).only('yelp')

## v0.5
* big refactoring from Rudy
* ready for releasing

## v0.3
* return hash instead of objects
* removing facets
* a little refactoring

## v0.2
* refactoring

## v0.1
* initial version
** a table agnostic read api, usage as: api.table(table_alias).rows
** normal (but powerful) filters, usage as: api.table(:global).filters(:country => {'$sw' => 'u'}, :region => 'ca')
** general mapping of ALL v3 api params, e.g. geo, query, sort, select, limit, offset
** places sugers, usage as: api.crosswalk(FACTUAL_ID); api.resolve(:name => 'factual inc.', :region => 'ca')
** facets
** different format, usage as: json_api = Factual::Api.new( KEY, SECRET, :json)
** immutable api objects
