public class Phrase
{
    private static String currentPhrase;

    /** Constructs a new Phrase object. */
    public Phrase(String p)
    {
         currentPhrase = p;
    }

    /** Returns the index of the nth occurrence of str in the current phrase;
     *  returns -1 if the nth occurrence does not exist.
     *  Precondition: str.length() > 0 and n > 0
     *  Postcondition: the current phrase is not modified.
     */
    public static int findNthOccurrence(String str, int n)
    {
        int loc = -1;
        int count = 1;
        String a = currentPhrase;
        while(a.indexOf(str)!=-1&&count!=n){
            loc = currentPhrase.length()-a.length()+a.indexOf(str);
            a = currentPhrase.substring(loc+1);
            count++;
        }
        return loc;
    }

    /** Modifies the current phrase by replacing the nth occurrence of str with repl.
     *  If the nth occurrence does not exist, the current phrase is unchanged.
     *  Precondition: str.length() > 0 and n > 0
     */
    public void replaceNthOccurrence(String str, int n, String repl)
    {
        String a = currentPhrase;
        int index = findNthOccurence(str,n);
        a = currentPhrase.substring(0,index) + repl +currentPhrase.substring(index+str.length());                   
                     
    }

    /** Return the index of the last occurrence of str in the current phrase;
     *  returns -1 if str is not found.
     *  Precondition: str.length() > 0
     *  Postcondition: the current phrase is not modified.
     */
    public int findLastOccurrence(String str)
    {
        int i = 1;
        int loc = -1;
        while(findNthOccurence(str,i)!=-1){
            loc = findNthOccurence(str,i);
            i++;
        }
        return loc;
    }
    /** Returns a string containing the current phrase */
    public String toString(){
        return currentPhrase;
    }
    public static void main(String[] args)
    {

    }
}
