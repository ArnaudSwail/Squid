


https://stackoverflow.com/questions/10929453/read-a-file-line-by-line-assigning-the-value-to-a-variable


```


# ------------------------------------------------------------------------------
#
# Nice treatment
#
# OLDIFS=$IFS
# IFS=";"
# while read user job uid location
#  do
#
#     echo -e "$user \
#     ======================\n\
#     Role :\t $job\n\
#     ID :\t $uid\n\
#     SITE :\t $location\n"
# done < $1
#  IFS=$OLDIFS


#while IFS='' read -r line || [[ -n "$line" ]]; do
#    # echo "Text read from file: $line"
#    variable=$1
#
#    for i in $(echo $variable | sed "s/;/ /g")
#    do
#        # call your procedure/other scripts here below
#
#        echo "$i"
#    done
#done < "$1"
```
