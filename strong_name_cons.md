#Scenarios where strong-naming is bad
====================
Add any scenarios where having/using strong-named open source assemblies cause problems for you as a 
user, developer, or contributor.

Remember: We're only considering the case where strong-named assemblies have the full strong-name key in the code
repository.

If possible, keep scenarios on separate lines and put your username, name or email at the end of your scenario.
If you want to respond to a scenario, place your response right after the scenario and indent by one

Example:

* Here is a scenario - username
  * A response to your suggestion - responder_username 


---------------
* "GAC-wins" could lead to unexpected binding. Let's say open source library LibA is
 strong-named with its strong naming key in its repo. A user, Pat, modifies LibA for own use but keeps the name, version
and key. If LibA is for some-reason in the GAC, it won't matter if Pat's assembly is in the app's folder, the GAC'd one
will always be used.
