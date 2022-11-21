# write-a-trigger-on-account-insert-two-account-record-using-the-recursion-concept-
write a trigger on account insert two account record using the recursion  concept 
account Trigger.apex
trigger mytrigger on Account(before update)
{
   if(trigger.isbefore && trigger.isupdate) 
        {
             AccountHandlers.afterinsert(trigger.new);
        }


}


//AccountHandlers.apx

public class AccountHandlers
{
    public static integer count=1;                     // initilaize count =1
}
  public static void afterinsert(List<Account> listacc)
     {
       list<Account> acclist=new afterinsert()


      if(recursionAvoid.isrecursion==true || count=1)
        {
           if(recursionAvoid.isrecursion==false)        
            {
              count++;
            }

            recursionAvoid.isrecursion=false;
           {
             for(account acc:acclist)
                {
                     Account accobj=new Account();
                     accobj.Name=acc.Name+'duplicate';
                     acclist.add(accobj);
                      
                   }

            if(acclist.isEmpty())
              {
                insert.acclist;
              }
           }
         }
      }





RecursionAVIlod
]public class RecursionAovid
{
   public static aBoolean isRecursion=true;
}
