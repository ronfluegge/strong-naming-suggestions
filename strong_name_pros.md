#Scenarios where strong-naming is good
----------------------------
Add any scenarios where having/using strong-named open source assemblies is good
for you as a user, developer, or contributor.

Remember: We're only considering the case where strong-named assemblies have the full strong-name key
in the code repository.

If possible, keep scenarios on separate lines and put your username, name or email at the end of your scenario.
If you want to respond to a scenario, place your response right after the scenario and indent by one.

Example:

* Here is a scenario - username
  * A response to your suggestion - responder_username

--------------------------------
* Strong-named open source libraries can be used by other strong-named libraries and applications. - ericschultz

--------------------------------

I always understood that:

1.Strong naming your assembly allows you to include your assembly into the Global Assembly Cache (GAC). Thus it allows you to share it among multiple applications.

2.Strong naming guarantees a unique name for that assembly. Thus no one else can use the same assembly name.

3.Strong name protect the version lineage of an assembly. A strong name can ensure that no one is able to produce a subsequent version of your assembly. Application users are ensured that a version of the assembly they are loading come from the same publisher that created the version the application was built with.

4.Strong named assemblies are signed with a digital signature. This protects the assembly from modification. Any tampering causes the verification process that occurs at assembly load time to fail. An exception is generated and the assembly is not loaded.
 
That's why we use them in GADS OS

 -- ronfluegge
