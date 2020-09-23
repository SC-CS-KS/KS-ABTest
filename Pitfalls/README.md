# A/B 实验的陷阱、疑难杂症

**低响应率现象**  

* 解决方案  

<table><tbody><tr><td width="123"><p><strong>破解方法</strong></p></td><td width="123"><p><strong>适用场景</strong></p></td><td width="113"><p><strong>优点</strong></p></td><td width="180"><p><strong>缺点</strong></p></td></tr><tr><td width="123"><p>1、反事实埋点法</p></td><td width="123"><p>广告投放的竞争机制带来的低响应率</p></td><td width="113"><p>一旦改造完成，可以一劳永逸。</p></td><td width="180"><p>需要繁琐的工程改造， 成本非常高。</p></td></tr><tr><td width="123"><p>2、基于倾向得分模型的样本纠偏方法</p></td><td width="123"><p>触达率较低导致的低响应率</p></td><td width="113"><p>提高响应率，一定程度减缓稀释影响</p></td><td width="180"><p>无法保证实验组和对照组的同质性，因此无法控制一类错误率，属于基于观察性实验的方法。</p></td></tr><tr><td width="123"><p>3、非依从因果推断框架☆☆重点推荐</p></td><td width="123"><p>所有的低响应率实验</p></td><td width="113"><p>不需要进行任何工程改造，适合观察到稀释问题后的事后补救</p></td><td width="180"><p>无</p></td></tr><tr><td width="123"><p data-spm-anchor-id="ata.13261165.0.i8.4d8e117eWUJ6XF">4、实验设计分流点后移（类似反事实埋点）</p></td><td width="123"><p>一般的低响应率实验</p></td><td width="113"><p>效果较好且可以叠加方法3</p></td><td width="180"><p>通用性较差</p></td></tr></tbody></table>


