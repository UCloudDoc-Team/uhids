{{indexmenu_n>5}}

# 主机漏洞

![](/images/operation/events/主机漏洞.png)

表1.主机漏洞列表参数

<table>
<thead>
<tr class="header">
<th>参数</th>
<th>说明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>主机IP</td>
<td>主机的IP地址，如果没有外网IP则显示为内网IP</td>
</tr>
<tr class="even">
<td>漏洞编号</td>
<td>漏洞的唯一编号</td>
</tr>
<tr class="odd">
<td>风险级别</td>
<td>根据风险类型评估的风险级别，包括「高危」、「中危」和「低危」</td>
</tr>
<tr class="even">
<td>应用类</td>
<td>此风险影响的应用范围是哪种，比如ntp</td>
</tr>
<tr class="odd">
<td>版本号</td>
<td>受影响的应用类的版本号</td>
</tr>
<tr class="even">
<td>处理状态</td>
<td>表示处理的状态，包括「未处理」和「已忽略」。<br />
如果已经处理了风险，则下次检测时将删除此风险信息。</td>
</tr>
</tbody>
</table>

**漏洞详情**

显示漏洞描述和如何处理漏洞的建议等。

<wrap
em>注意：漏洞修复属于高风险操作，务必做好风险规避，妥善实施漏洞修复！</wrap>参见此处了解[如何修复漏洞](/security/uhids/faq/bugs)？

**忽略**

<wrap em>注意：点击【忽略】且确认后，此主机IP的此种风险类型将不再进行检查。并且无法取消忽略。</wrap>
