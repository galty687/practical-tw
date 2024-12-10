# DITA 快速入门

## DITA Topic 类型

DITA认为技术信息的基本构成单位是 Topic ，而 Topic 根据其使用目的又可以分为以下四类：

- Task。如何做某件事，例如，如何启动投影仪；
- Concept。介绍某个概念或实物，例如，什么是VGA接口；
- Reference。介绍具体参数信息，例如投影仪灯泡的规格、API接口等；
- Troubleshooting。介绍如何排除故障，例如，无法启动投影仪怎么办；

## 新建 Concept 主题

Concept Topic 基本结构

```
        - title
          - shortdesc
          - conbody
        - p (optional)
        - section
            - title
        - p
        - image
        - codeblock
        - etc.
```

这里演示如何 使用oXygen XML 24 创建Concept.

## 新建 Task 主题

```
-task
-title
-shortdesc
- taskbody
     - prereq
     - context
     - stepsection
     - steps
          - step
               -cmd
               - info
                    - note
                    - image
                    - codeblock
               - stepxmp
               - stepresult
               - choices
               - substeps
     - result
     - example
     - postreq
```

## 新建 Reference 主题

## 新建 Troubleshooting 主题

## 使用 DITAMAP 创建输出
