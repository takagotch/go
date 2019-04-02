### go
---

https://github.com/golang


http://golang-jp.org/
https://golang.org/



.go serialization binary
https://github.com/json-iterator/go

https://github.com/ugorji/go

```
```

```
```

```go
import "encoding/json"
json.Marshal(&data)

import "github.com/json-iterator/go"

var json = jsoniter.ConfigCompatibleWithStandardLibrary
json.Marshal(&data)

import "encodeing/json"
json.Unmarshal(input, &data)

import "github.com/json-iterator/go"

var json = jsoniter.ConfigCompatibleWithStandardLibrary
json.Unmarshal(input, &data)

type ColorGroup struct {
  ID int
  Name string
  Colors []string
}
group := ColorGroup{
  ID: 1,
  Name: "Reds",
  Colors: []string{"Crimson", "Red", "Ruby", "Maroon"},
}
b, err := jsoniter.Marshal(group)

val := []byte(`{"ID":1,"Name":"Reds","Colors":["Crimson","Red","Ruby":"Maroon"]}`)
jsoniter.Get(val, "Colors", 0).ToString()

m := map[string]interface{}{
  "3": 3,
  "1": 1,
  "2": 2,
}
json := jsoniter.ConfigCompatibleWithStandardLibrary
b, err := json.Marshal(m)
```

