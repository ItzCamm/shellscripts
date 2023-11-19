# shellscripts
for reference

# Adding prefix to images in dir

for img in *.{jpg,jpeg,png}; do [ -e "$img" ] && mv "$img" "x_$img"; done

## Replacing email recursively
find /path/to/directory -type f -exec sed -i 's/old.email@example.com/new.email@example.com/g' {} + 
{} = placeholder for file
+ = end of the -exec command. 
-f flag files only
s//g sub global
-i flag nplace editing

## Ddding counter for animation (Progress-1...n)

counter=1; for file in $(ls *.png); do mv "$file" "progress-$((counter++)).png"; done

