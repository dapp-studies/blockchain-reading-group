### Blockchain Reading Group

<p>

Blockchains, cryptocurrencies, and contracts are a source of far more
problems than can be handled by developer communities and investors
currently driving their adoption.

As it stands, a multi-billion market capitalization rests in the hands of a growing
collection of developers that cannot honestly tell you they have everything under control.

We can help bridge the gap by reading and discussing notable academic research in an informal setting.


I've included the 167 e-prints on the <a href="https://arxiv.org">arXiv</a> on the topic of blockchain, so we have some selection [but not that much - 48.8% are on Cryptography and Security, and only 18 cover Ethereum].

</p>


##### Suggestions for Week 1

<ul>
<li> <a href="http://arxiv.org/pdf/1702.05511v1">A Concurrent Perspective on Smart Contracts</a></li>
<li><a href="http://arxiv.org/pdf/1703.03779v1">Dissecting Ponzi Schemes on Ethereum</a></li>

</ul>


Please leave any suggestions of your own below.


***



<div id="_container""></div>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script type="text/javascript">
	$('document').ready(function () 
	{
		entries.forEach((entry) => 
		{
			var d = document.createElement('div');
			d.innerHTML =
			`
			<div class="ui centered segment">
				<div class="title">
					<a href="${entry.pdf_link}"><h4>${entry.title}</h4></a>
				</div>
 		      <div class="meta">
			      	<span>${entry.author}, ${(new Date(entry.published)).toString().substring(0,16)}</span>
			      	<br/>
			      	&nbsp;
			      	<emph>${entry.primary_category}</emph>
	   		</div>
			    <div class="content">
						<div class="ui accordion">
							<div class="title">
						    	<i class="dropdown icon"></i>
						    	Abstract
						    </div>
						    <div class="content"">
							    <p class="transition hidden">${entry.abstract}</p>
							</div>
					  </div>
			    </div>
			</div>
		<div class="ui hidden divider"></div>`;
		$("#_container")[0].appendChild(d);
		});
		$('.ui.accordion').accordion();
	});
</script>
