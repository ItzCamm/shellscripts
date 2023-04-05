# shellscripts
for reference

#Adding prefix to images in dir
for img in *.{jpg,jpeg,png}; do [ -e "$img" ] && mv "$img" "x_$img"; done
