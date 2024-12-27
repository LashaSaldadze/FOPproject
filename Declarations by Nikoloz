import java.util.HashMap;
import java.util.List;
import java.util.Map;
import java.util.Scanner;
import java.util.ArrayList;

public class BasicJavaInetrpreter {

    public static void main(String[] args) {
    	String code = "Placeholder code here";
    	String[] lines = code.split("\\n");}; // splits code between lines
    	Map<String, String> declaredValues = new HashMap<>();
    	
    	public void declareVariable(String[] lines) {
        for (String line : lines) {
    	    line = line.trim();
            if (line.isEmpty()) continue;

            if (line.startsWith("LET "))   // Variable declaration or assignment
        	    line = line.substring(4); // Remove "LET "
                String[] parts = line.split("="); //splitting variable name and variable value
                String varName = parts[0].trim();
                String varValue = parts[1].trim();
                declaredValues.put(varName, varValue); //adding name and value pairs to our map for later use
                //Here should be a way to figure out how to check if value is secretly an int or float
                   
        }       
    	}
       
    }

