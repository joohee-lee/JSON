# JSON  
:  JSON (JavaScript Object Notation) 

JSON (JavaScript Object Notation) is quite possibly the most widely used data format for data interchange on the web. It has likely surpassed XML (which is used in AJAX applications) as the most common format used for asynchronous browser/server communication.
- 웹에서 데이터 교환에 가장 널리 사용되는 데이터 형식입니다. 비동기 브라우저 / 서버 통신에 사용되는 가장 일반적인 형식으로 XML (AJAX 애플리케이션에서 사용)을 능가했을 것입니다.

JSON is a human and machine readable format
- JSON은 사람이 읽고 읽을 수있는 형식입니다.

JSON is based on a subset of JavaScript

JSON was inspired by the object literals of JavaScript (also known as ECMAScript). However, despite this, JSON is language-agnostic. It can facilitate data interchange between most, if not all programming languages. In fact, JSON uses common programming conventions, which makes it familiar to most programmers, regardless of their chosen language/s.
- JSON은 JavaScript의 객체 리터럴 (ECMAScript라고도 함)에서 영감을 얻었습니다. 그러나 그럼에도 불구하고 JSON은 언어에 구애받지 않습니다. 모든 프로그래밍 언어는 아니지만 대부분의 데이터를 쉽게 교환 할 수 있습니다. 실제로 JSON은 일반적인 프로그래밍 규칙을 사용하므로 선택한 언어에 관계없이 대부분의 프로그래머에게 친숙합니다.


1.   JSON  Obj   
```
{ key : value}
{ "artistname" : "deep purple"}
{
    "aritstname" : "deep purple";
    "formed" : "1968"
}
{
   "artistname" : "Deep Purple", 
  "formed" : "1968",
  "origin" : "Hertford, United Kingdom"
}

```

2.   JSON  Array

-  2.1  JSON  Array
A JSON array is an ordered collection of values. It allows you to provide a list of values.
JSON 배열은 정렬 된 값 모음입니다. 값 목록을 제공 할 수 있습니다.

```

{
    "artists" : [
        {
            "artistname" : "Deep purple",
            "formed" : "1968"
        },
        {
            "artistname" : "Joe Satriani",
            "formed" : "1968"
        },
        {
            "artistname" : "Maroon 5",
            "formed" : "1994"
        
        }
    ]
}

```

-  2.2  White Space
: 공백을 사용하여 JSON 문서를 더 읽기 쉽게 만들 수 있습니다. 실제로 이것은 JSON 및 대부분의 프로그래밍 언어와의 공통 규칙입니다.

```
{
    "artists" : [
        { "artistname" : "Deep purple", "formed" : "1968" },
        { "artistname" : "Joe Satriani", "formed" : "1968" },
        { "artistname" : "Maroon 5", "formed" : "1994" }
    ]
}

```

- 2.3 Nested Data
Most JSON files contain lots of nested data. This is driven by the structure of the data.
대부분의 JSON 파일에는 많은 중첩 데이터가 포함됩니다. 이는 데이터 구조에 의해 결정됩니다.

ex1)

```

{
    "artists" : [
        {
            "artistname" : "Deep purple",
            "formed" : "2968",
            "albums" : [ 
                {
                    "albumname" : "Machine Head",
                    "year" : "1972",
                    "genre" : "Rock"
                }, 
                {
                    "albumname" : "Stormbringer",
                    "year" : "1974",
                    "genre" : "Rock"
                }
            ]
            
        }
    ]
}

```

ex2)

```
{
    "artists" : [
        {
            "artistname" : "Deep purple",
            "formed" : "1968",
            "albums" : [
                { 
                    "albumnamne" : "Machine Head",
                    "year" : "1972",
                    "genre" : "Rock"
                },
                {
                    "albumnamne" : "Stormbringer",
                    "year" : "1972",
                    "genre" : "Rock"
                }
            ]
        },
        {
            "artistname" : "Joe Satriani",
            "formed" : "1956",
            "albums" : [
                { 
                    "albumnamne" : "Flying in a Blue Dream",
                    "year" : "1989",
                     "genre" : "Instrumental Rock"
                },
                {
                    "albumnamne" : "The Extremist",
                    "year" : "1992",
                     "genre" : "Instrumental Rock"
                }
            ]
        }
    ]
}

```



