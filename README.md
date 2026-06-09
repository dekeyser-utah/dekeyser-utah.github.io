# Description
Static page to promote our house in Normandie, France.
Deployed on github pages at https://dekeyser-utah.github.io/


# thumb and resize staand
for f in *.JPG; \
do 
    convert -resize 600x400 $f resized-$f
    convert -thumbnail 90 $f thumb.$f
done



# local setup
```
python3 -m http.server 8000
```
Required for the youtube iframe to work.