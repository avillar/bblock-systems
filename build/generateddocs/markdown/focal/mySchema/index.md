
# My Schema (Schema)

`ogc.focal.mySchema` *v0.1*

An example schema defining the set of properties of any type of object.

[*Status*](http://www.opengis.net/def/status): Under development

## Description

## My Schema

Defines a set of properties that may be used in **any** JSON schema.

> Note these properties may be used in the "properties" sub-component of a GeoJSON object, as a simple object

The numeric properties "b" and "c" have an example SHACL rule that if c is present, then c > b
## Examples

### This is an example with just a description and no code snippets.
This an example.

In **Markdown** format.
#### json
```json
{
  "LT": "2S1",
  "LES_OBL": 8,
  "LO_CAST": "a",
  "UDRZBA": 2022,
  "ZMENA": "Uvedení do souladu s KN",
  "ZADOST": "-",
  "CHS": 25,
  "PCHS": "25a",
  "OVER_T": "NE",
  "ROK_MAP": 2015,
  "ID1": 128301,
  "SLT": "2S",
  "PLOCHA": 1224.24963,
  "DS_OPRL": 2025
}


```

#### jsonld
```jsonld
{
  "@context": [
    {
      "mynamespace": "http://example.com/mythings/"
    },
    "https://markuswilhelmjahn.github.io/bblock-systems/build/annotated/focal/mySchema/context.jsonld"
  ],
  "LT": "2S1",
  "LES_OBL": 8,
  "LO_CAST": "a",
  "UDRZBA": 2022,
  "ZMENA": "Uveden\u00ed do souladu s KN",
  "ZADOST": "-",
  "CHS": 25,
  "PCHS": "25a",
  "OVER_T": "NE",
  "ROK_MAP": 2015,
  "ID1": 128301,
  "SLT": "2S",
  "PLOCHA": 1224.24963,
  "DS_OPRL": 2025
}
```

#### ttl
```ttl
@prefix focal-prop: <https://w3id.org/ogc/hosted/focal/properties/> .

[] focal-prop:lesniTyp <https://w3id.org/ogc/hosted/focal/lt/2S1> .


```


### Examples can have content and/or code snippets.
The content of this example. 
#### shell
```shell
echo 'Hello, world!'
```

#### python
```python
print('Hello, world!')
```

#### javascript
```javascript
console.log('Hello, world!')
```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: My example schema
type: object
properties:
  LT:
    type: string
    x-jsonld-id: https://w3id.org/ogc/hosted/focal/properties/lesniTyp
    x-jsonld-type: '@id'
    x-jsonld-base: https://w3id.org/ogc/hosted/focal/lt/
  LES_OBL:
    type: number
  LO_CAST:
    type: string
  UDRZBA:
    type: number
  ZMENA:
    type: string
  ZADOST:
    type: string
  CHS:
    type: number
  PCHS:
    type: string
  OVER_T:
    type: string
  ROK_MAP:
    type: number
  ID1:
    type: number
  SLT:
    type: string
  PLOCHA:
    type: number
  DS_OPRL:
    type: number
required:
- LT
x-jsonld-prefixes:
  focal-prop: https://w3id.org/ogc/hosted/focal/properties/

```

Links to the schema:

* YAML version: [schema.yaml](https://markuswilhelmjahn.github.io/bblock-systems/build/annotated/focal/mySchema/schema.json)
* JSON version: [schema.json](https://markuswilhelmjahn.github.io/bblock-systems/build/annotated/focal/mySchema/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "LT": {
      "@context": {
        "@base": "https://w3id.org/ogc/hosted/focal/lt/"
      },
      "@id": "focal-prop:lesniTyp",
      "@type": "@id"
    },
    "focal-prop": "https://w3id.org/ogc/hosted/focal/properties/",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://markuswilhelmjahn.github.io/bblock-systems/build/annotated/focal/mySchema/context.jsonld)

## Sources

* [Sample source document](https://example.com/sources/1)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/MarkusWilhelmJahn/bblock-systems](https://github.com/MarkusWilhelmJahn/bblock-systems)
* Path: `_sources/mySchema`

