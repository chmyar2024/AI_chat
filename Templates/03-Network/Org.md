---
# === 核心属性 ===
type: org
mode: quick
status: active
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/org]

# === 扩展属性 ===
org_type: ""        # company/community/institution
industry: ""
relationship: ""    # employer/client/partner/customer
related: []
---

> [!abstract] Org: 组织机构管理
> **用途**: 管理公司、社区、机构等组织关系

---

## 🏢 组织信息

**名称**: <%tp.file.cursor(1)%>

**类型**: `= this.org_type`  
**行业**: `= this.industry`  
**关系**: `= this.relationship`

---

## 📝 基本信息

**简介**: 
> 

**规模**: 
**网站**: 

---

## 👥 关键联系人

```dataview
LIST FROM "03-Network/Person"
WHERE up = this.file.link
```

### 快速添加
- [[03-Network/Person/<%tp.file.cursor(2)%>|]]

---

## 🤝 合作情况

### 当前合作
- [[05-Execution/Project/]]

### 历史合作
- 

---

## 📊 组织画像

**优势**: 
- 

**文化**: 
- 

**机会**: 
- 

---

## 🔗 相关链接

**相关项目**: [[05-Execution/Project/]]  
**相关人员**: [[03-Network/Person/]]  
**相关资源**: [[03-Network/Resource/]]
