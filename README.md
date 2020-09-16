# PhpStormSettings
This is my own php storm setting with some live template that I think is usefull.

Here live template description :

- [*dataProvider*] 

This live template is for auto generate a dataProvider blueprint with documentation. Because I get lazy to type it or copy/past from other phpunit test.

- [*@paramRequest*] 

This one is for auto generate a pre-writen documentation for request parameter. Because it does not seams to exist a standard way to document request parameter (Also look those SO posts http://tiny.cc/4uiwsz, http://tiny.cc/1uiwsz).
(Notice that in the following example I use the Request service from Symfony framework, so I can use it as a @param)
I use it like that : 
```
  * @param Request $request
  * <ul>
  *  <li><i>string</i> $_GET['<b>selected_group_code</b>'] <i>(optional)</i> group code</li>
  *  <li><i>string</i> $_GET['<b>selected_page_number</b>'] <i>(optional)</i> page number</li>
  *  <li><i>string</i> $_GET['<b>selected_label_product</b>'] <i>(optional)</i> product label</li>
  * </ul>
  public function listProduct(Request $request){
  ...
  }
```
I think it's good enough for a documentation purpose...
