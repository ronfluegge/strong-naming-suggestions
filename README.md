Gaye Oncul Kok of the Microsoft .Net Framework team and I are collaborating on creating best practices 
for strong-naming of open source .Net assemblies. We have two possible recommendations for open source libraries: 

1.	Strong name assemblies and place the full strong-naming key in your public repository 
[strong_name_pros.md](strong_name_pros.md)    
2.	Don’t strong-name assemblies [strong_name_cons.md](strong_name_cons.md)    

I know there are advantages and disadvantages to each but we’d like to know which ones you know of. 
Please fork this repository and provide your feedback so we can provide the best possible recommendation.

Note: we're really asking just for issues with libraries. We've concluded that .exe assemblies shouldn't be strong-named
in most cases.
