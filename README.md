# JS-loading
JS实现简单loading功能页面


              <html>  
              <head>  
              <title>正在载入...</title>  
              <meta http-equiv="Content-Type" content="text/html; charset=gb2312">  
              </head>  
              <body bgcolor="#FFFFFF" leftmargin="0" topmargin="0">  
              <table border=0 cellpadding=0 cellspacing=0 width="100%" height="100%">  
              <tr>   
              <form name=loading>  
              <td align=center>   
              <p><font color=gray>正在载入首页，请稍候.......</font></p>  
              <p>   
              <input type=text name=chart size=46 style="font-family:Arial;   
              font-weight:bolder; color:gray;  
               background-color:white; padding:0px; border-style:none;">  
              <br>  
              <input type=text name=percent size=46 style="font-family:Arial;   
              color:gray; text-align:center;   
              border-width:medium; border-style:none;">  
              <script>var bar = 0   
              var line = "||"   
              var amount ="||"   
              count()   
              function count(){   
              bar= bar+2   
              amount =amount + line   
              document.loading.chart.value=amount   
              document.loading.percent.value=bar+"%"   
              if (bar<99)   
              {setTimeout("count()",100);}   
              else   
              {window.location = "http://blog.csdn.net/miner_lee";}   
              }  
              </script>  
              </p>  
              </td>  
              </form>  
              </tr>  
              </table>  
              </body>  
              </html>  



