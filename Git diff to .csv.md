```
diff -u template_material2_only.html template_neither.html \
  | grep -e '^+' -e '^-' \
  | grep -v '^+++' \
  | grep -v '^---' \
  | sed 's/^+\(.*\)/Added,\1/; s/^-\(.*\)/Removed,\1/' > diff.csv
```