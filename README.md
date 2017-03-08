procedure TForm1.btn1Click(Sender: TObject);  
var    doc:olevariant;    str:string;  
begin      
doc:=wb1.Document;      //获取元素的值      
{str:=doc.all.xx.value;     ShowMessage(str);}        
//写入htnl      
{doc.clear;     doc.write('<html><head></head><body><p>新的html</p><input type="hidden" value="0" id="xx" /></body></html>');     
doc.close;}        //改变元素的值      
{doc.all.xx.value:='1';     ShowMessage(doc.all.xx.value);}        
//获得html文本      {str:=doc.documentElement.outerHtml;     ShowMessage(str);}        
//触发元素的事件      {doc.all.bt.onclick;}        
//执行js      wb1.OleObject.document.parentWindow.execScript('aa()','JavaScript');  
end;  
