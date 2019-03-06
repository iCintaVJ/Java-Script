<script>
var a=prompt("Enter your Co-Ordinates", "110°4\'21\"W");
var b=prompt("Enter your Co-Ordinates", "110°4\'21\"W");
var lon=dms(a);
var lat=dms(b);
document.writeln(lon);
document.writeln(lat);
function dms(val){
var str=val.toLowerCase();
var d=str.substring(0,str.indexOf('°'));
var m="";
var s="";
for(var i=str.indexOf("°"); i<str.length; i++){
    var temp=str.charAt(i);
    if((str.charAt(i)>='0' && str.charAt(i)<='9')||(str.charAt(i)=='\.')){
        m+=temp;
    }
    if(str.charAt(i)=='\''){
        break;
    }
}
for(var i=str.indexOf("\'"); i<str.length; i++){
    var temp=str.charAt(i);
    if((str.charAt(i)>='0' && str.charAt(i)<='9')||(str.charAt(i)=='\.')){
        s+=temp;
    }
    if(str.charAt(i)=='\"'){
        break;
    }
}
var dd=parseInt(d,10);
var mm=parseInt(m,10);
var ss=parseInt(s,10);
var res=dd+(mm/60)+(ss/3600);
if(str.charAt(0)=='-'){
    if(str.charAt((str.length)-1)=='w' || str.charAt((str.length)-1)=='s'){
        res= -(res);
    }
}
else{
    if(str.charAt((str.length)-1)=='e' || str.charAt((str.length)-1)=='n'){
        res= -(res);
    }
}
return res;
}
</script>
