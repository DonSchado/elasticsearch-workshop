### Elasticsearch Example

`rake db:create && rake db:migrate`

`rake db:seed` will generate about 1000 articles and index about 10000 documents

---

otherwise or in case of errors you can rebuild the index from the console:

```
  >> Article.__elasticsearch__.create_index! force: true
  => {"acknowledged"=>true}
  >> Article.import
  => 0
  >>
```
