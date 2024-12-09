# Troubleshooting

## 故障

只要用户开始使用产品就会遇到故障，很多用户看手册是要寻找解决问题的信息。[根据 Lazonder 等人的研究](https://research.utwente.nl/en/publications/the-effect-of-error-information-in-tutorial-documentation)，用户25%的时间是在应对各类错误。

## 故障排除信息

### 结构

| 元素         | 目的                 | 示例                             |
| ------------ | -------------------- | -------------------------------- |
| 故障识别     | 让用户知道错误的存在 | DITA 输出中文乱码                |
| 故障分析     | 描述错误的原因       | 未指定xml的语言为中文            |
| 故障排除方法 | 提供解决故障的方式   | 在map元素中增加 xml:lang="zh_CN" |

### 建模
| 元素              | 含义           |
| ----------------- | -------------- |
| `<troubleshooting>` |                |
| `<title>`           | 故障识别       |
| `<condition>`       | 故障发生的条件 |
| `<cause>`           | 诊断           |
| `<remedy>`          | 故障排除方法   |

## 写作风格

### `<title>`

1. 使用用户最有可能描述问题的方式来写标题。
2. 增加 `<indexterms>`方便搜索。



## 示例

来自dita.xml.org的对各元素的说明

```xml
<?xml version="1.0" encoding="utf-8"?>
<!DOCTYPE troubleshooting
  PUBLIC "-//OASIS//DTD DITA Troubleshooting//EN"
  "troubleshooting.dtd">
<troubleshooting id="REPLACE_THIS">
  <title><!-- State the essential nature of the problem --></title>
  <shortdesc><!-- Be more specific about the problem here --></shortdesc>
  <prolog>
    <metadata>
      <keywords><!--
          Make sure to use indexterms. Readers often find troubleshooting content through the index.
          Provide indexterm variants that readers might use. For example:
        <indexterm>Logon
          <indexterm>troubleshooting</indexterm>
        </indexterm>
        <indexterm>troubleshooting
          <indexterm>Logon</indexterm>
        </indexterm>
        -->
      </keywords>
    </metadata>
  </prolog>
  <troublebody>
    <condition><!--
        The topic title and the shortdesc should have already told your reader a lot about the
        condition that this topic seeks to fix. Use condition to expand upon that. Do not simply
        repeat what you have already put into the title and the shortdesc. Condition is the
        appropriate place to put impact and severity information. If multiple solutions exist and
        their relationships with each other are complex, you can discuss that here.-->
      <title><!-- Optional title. Use "Condition". --></title>
      <p></p>
    </condition>
    <troubleSolution><!--
        troubleSolution is meant to hold pairs of cause and remedy. Occassionally, you might have
        cause without remedy or remedy without cause, but that should be rare. Be sure to order
        mutliple troubleSolution elements in a sequence that makes sense. For example, order them
        by the likelihood of a cause occuring. You may wish to deviate from that if a remedy for a
        less likely cause is much easier to try. Remember to use conref for troubleSolution
        elements that are the same across multiple troubleshooting topics.-->
      <cause>
        <title><!--
          Optional title. Use "Cause". For topics with mutliple troubleSolutions, state the
          essential nature of this particular cause instead of just using "Cause".-->
        </title>
        <p></p>
      </cause>
      <remedy>
        <title><!-- Optional title. Use "Remedy" or "Solution". -->
        </title>
        <responsibleParty><!--
          Optional. Use this element to indicate the role of who ought to be performing the steps
          in the remedy. Here are some examples: "engineer", "customer", "field-support".
        -->
        </responsibleParty>
        <!-- You can use steps-unordered or steps-informal instead of steps. -->
        <steps>
          <!-- 
               Remember that you can use conref to bring in steps from tasks or other
               troubleshooting topics. -->
          <step>
            <cmd/>
          </step>
        </steps>
      </remedy>
    </troubleSolution>
  </troublebody>
</troubleshooting>
```