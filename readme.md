# Day one 16.11.

## Fabien (keynote)

* composer req master
* symfony/lts
* api platform 

## Decoupling applications with message queues

* amqp
* UX paremmaksi, nopeat responset käyttäjälle
* event handlereiden käytössä ?
* bernard "poor man's queues"

## From legacy to Symfony

* kuinka käyttää symfony 4.0 legacy softissa
* LegacyBundle, check GoldenLine GitHub
* ottivat legacy softassa symfony 2.1 käyttöön
  * käyätnnössä kaikki liikenne symfonyn läpi wanhaan softaa
  * tekivät @LegacyXXX annotaatiot hanskaamiseen
    * käytäjärooli
    * OldBrowser
* varnish
* esi

## Building your translation process

* external source for translations
  * loco (ui + api)
* xliff
* how to deploy translations ?
* php-translation.readthedocs.io
* context for key
* PHP-translation (gui, extractor, saad integration, autofallback) <-- check this
* JMSTranslatorBundle
* LexikTranslationBundle

## Building a cloud-friendly application 

* platform.sh
* readonly filesystem
* divide code and context / content
* DI your environment
  * DB credentials
  * API keys
  * paths on disk
  * domain names
* glue code to process / parse env variables in different environments aws, heroku, etc

## Discovering & solving performance issues

* JMeter - load & capacity testing
* HTTPlug
* profiler in functional test, see symfony docs
* github.com/phan/phan
* caching in symfony: an overview denis brumann


## composer.lock

* checkout masterin coposer.lock filusta
* after that compser update


## Lessons learned building the composer internals (keynote)

# Day two 17.11.

## PHP 7.2 and beyond

* puhuja php 7.2 julkaisun hyväksyjä
* packagistin mukaan 2/3 käyttäjistä käyttää php 7.x
* julkistus 13 päivän päästä
* tulevaisuus
  * retry poikkeuksiin
  * JIT
  
## Mastering regex incantations

* tsekkaa aina kaikki suunnat, A4Z /A(?=\d)\d(?<\d)Z/
* conditional groups
* recursiot (?R)
* subroutines (?(DEFINE))
* multiline käytä aina \A regex \Z
* shortcode see github
* regular-expression.info
* rexegg
* github.com/thunderer

## API Platform

* ranskalainen heppu ei kovin selkeä seurata :)

## Dependency injection v4

* _instaceof service conffeissa
* arguments:
  - !tagged foo
* %env(file:API_KEY_FILE)%
* secretir filuihin
* ServiceSubscriberInterface
* strict mode autowireen

## Doctrine performance

* seedien käyttö tietokannan täyttöön testejä varten
* faker composer
* testaa testaa ja testaa

## A year of symfony

* prefix route annotations
* debug:autowiring
* CoverageListener
* argon2i password hasher
* environmnet variables int: bool: float: file: json: base64:
* mahdollisuus luoda env variable conffeissa env(FOO): 'bar'
* minimalist-psr-3-logger
* bundle support tsekkaa lista

## Symfony community awards






