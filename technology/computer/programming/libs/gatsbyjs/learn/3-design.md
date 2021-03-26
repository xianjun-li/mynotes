---
slug: "design-flow"
date: "2021-03-08"
draft: true

title: "设计流程"
description: ""
categories:
  - "technology/computer/programming/lib/gatsbyjs"
series:
  - "gatsbyjs"
---

# 设计

## 0. 主要流程

参考: <https://www.gatsbyjs.org/docs/programmatically-create-pages-from-data/>

1. 在`gatsby-config`配置插件
2. 设计模板
3. `gatsby-node.js` 从数据源查询数据，将数据注入到模板
4. 模板内部流程
   - 模板本身的查询
   - 模板填入数据
   - 生成页面

## 1. 配置插件：

略

## 2. 模板

```jsx
// template
export default function Template(data) {
  // ...
}

// page query: graphql query
export const pageQuery = graphql`...`;
```
