<pre><code class="python" contentEditable="true">
import unicodedata

x = input("Diga-me a estação que deseja fazer a compra: \n")

x = unicodedata.normalize('NFKD', x).encode('ascii', 'ignore').decode('utf8')

if x.lower() == "verao":
  print("StreamShop,","R$89,99")    
elif x.lower() == "primavera":
  print("Loajing,", "R$84,00")    
elif x.lower() == "outono":
  print("Showpping,", "R$73,00")    
elif x.lower() == "inverno":
  print("Loajing,", "R$139,00")    
else:
  print("Valor inválido")
</code></pre>
