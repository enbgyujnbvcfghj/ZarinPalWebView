# ZarinPalWebView



Guide To using this module
To use this module, Do the following:
1- Put the PHP files that are included with the module on your site. And in the last character of the address there Is no / .
2- Add L_ZarinPal_Payment Layout To the Designer.
3- Add libraries (HttpUtils2, RichString, StringUtils, StatusBarCompat, JISON, IME, phone).
4- In the Module's Initialize, be sure to enter the required items.
5- Place the following code where you want To call the module.

  ZarinPal_Payment.money = "101" 'MONEY
  ZarinPal_Payment.Description = "Hello to you" 'Description
  ZarinPal_Payment.E_Mail = "a.hassanzadeh.1381@gmail.com" 'Mail
  ZarinPal_Payment.phone = "09152079018" 'phone
  ZarinPal_Payment.Activity_Now = Me 'don't change this Line
  StartActivity (ZarinPal_Payment)

6- put the same in the same part.
  Sub Zarin_Pal_Request( Status As String, Kod_Payment As String)
    'اگر ستاتوس برابر 100 يا 101 بود تراکنش موفق بوده!
    'اگر استاتوس برابر تال يا ... بود تراکنش ناموفق
    Msgbox("وضعيت تراکنش: "&Status& CRLF&"کد پيگيري تراکنش: " & Kod_Payment ,"")
    Log(Status& CRLF & Kod_Payment)
  End Sub

To contact support, email the following message. (programingcenter.97@gmail.com)
