# DITA 深入了解

## 内容复用

1. 将需要复用的文本片段存储再 `snippets.dita`中

2. 在需要复用的地方使用 `file name#topic_id/element_id`进行内容复用

例如：



Snippets.dita 片段中的提示信息

```xml
<topic id="topic_slh_bsm_lrb">
    <title>snippets</title>
    <body>
        <note id="reminder">可能会有微小误差，在国家标准之内</note>
    </body>
</topic>

```

在projector_spec.dita中引用上方提示信息

```xml
            <strow>
                <stentry>
                    <p>光圈范围</p>
                </stentry>
                <stentry>
                    <p>F=1.75-2.42</p>
                    <note conref="snippets.dita#topic_slh_bsm_lrb/reminder"/>
                </stentry>
            </strow>
```



## 文本链接

- **Hierarchical links** 。文档结构。`<topicref>`
- **inline links**. 文内超链接。`<xref>`
- **Related Links**.相关链接



### 相关链接

#### 直接添加

```
<related-links>
    <link href="sample1.dita"><linktext>Sample 1 Page</linktext></link>
    <link href="sample2.dita"/>
    <link href="sample3.dita"/>
 </related-links>
```

#### 关系表

```
    <reltable>
      <relheader>
   <relcolspec type="concept">
   <relcolspec type="task">
   <relcolspec type="reference">
      </relheader>
     
      <relrow>
        <relcell>
          <topicref href="sample_concept.dita"/>
        </relcell>
      
        <relcell>
          <topicref href="task_example1.dita"/>
          <topicref href="task_example2.dita"/>
        </relcell>

        <relcell>
          <topicref href="referencefile.dita"/>
         </relcell>
      </relrow>
    </reltable>
```
## 相关资源

- [DITA Notes](https://idratherbewriting.com/ditaval/)

