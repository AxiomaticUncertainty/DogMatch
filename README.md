# DogMatch
Dog Rating/Adoption App and Image API

https://www.dogmatch.app/

## API Base
```
https://www.dogmatch.app/api/v1
```

## Commands

### List Breeds
```
GET /breeds
```
Response:
```JSON
{
"status": 200, 
"breeds": ["Affenpinscher", "Afghan Hound", ..., "Yorkshire Terrier"]
}
```

### Get Random Breed
```
GET /breeds/random
```
Response:
```JSON
{
  "status":200,
  "breed":"German Short-haired Pointer"
}
```

### Check if Breed Is in Dataset
```
GET /breeds/:breed
```
Response:
```JSON
{
  "status":200,
  "contains":true
}
```

### Get Image for Breed
```
GET /breeds/:breed/image
```
Response:
```JSON
{
  "status":200,
  "image":"https://dogmatch.app/api/v1/images/Siberian Husky/n02110185_3540.jpg"
}
```

### Get Number of Images for Breed
```
GET /breeds/:breed/count
```
Response:
```JSON
{
  "Status":200,
  "Count":192
}
```
