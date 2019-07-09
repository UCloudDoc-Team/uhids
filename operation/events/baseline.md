{{indexmenu_n>1}}

# 安全基线检查

![](/images/operation/events/安全基线检查.png)

表1.安全基线检查列表参数

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
<td>风险级别</td>
<td>根据风险类型评估的风险级别，包括「高危」、「中危」和「低危」</td>
</tr>
<tr class="odd">
<td>风险类型</td>
<td>检测出的风险类型，比如配置缺陷，点击操作中的【风险详情】可以查看更多描述</td>
</tr>
<tr class="even">
<td>应用类</td>
<td>此风险影响的应用范围是哪种，比如linux操作系统</td>
</tr>
<tr class="odd">
<td>风险描述</td>
<td>描述为什么判断为风险</td>
</tr>
<tr class="even">
<td>处理建议</td>
<td>为主机所有者提供处理此风险的建议</td>
</tr>
<tr class="odd">
<td>处理状态</td>
<td>表示处理的状态，包括「未处理」、「检查中」和「已忽略」。<br />
如果已经处理了风险，则下次检测时将删除此风险信息。<br />
如果希望立即检查，则可以点击【检查】按钮</td>
</tr>
</tbody>
</table>

**风险详情**

![](/images/operation/events/风险详情.png)

**忽略**

<wrap em>注意：点击【忽略】且确认后，此主机IP的此种风险类型将不再进行检查。并且无法取消忽略。</wrap>

**检查**

修复过风险，但是风险仍然处于「未处理」状态，可以通过立即检查让系统确认风险是否已经解决。如果风险已经解决则将看不到风险提醒信息。
