# FlexSim

### Convenyor - para enviar quando o processador estiver disponível
```
Conveyor.DecisionPoint current = ownerobject(c);
Object item = param(1);
Conveyor conveyor = param(2);
Conveyor.Item conveyorItem = conveyor.itemData[item];

// If this function returns a true, the default draw code of the object will not be executed.
{ //************* PickOption Start *************\\
/***popup:Conveyor_SendItem*/
/**Send Item*/

if (/**\nCondition: *//***tag:condition*//**/Model.find("Torrador 1").as(Object).stats.state().valueString == "idle"/**/) {
	/**\nDestination: */
	treenode newDest = /***tag:destination*//**/current.outObjects[1]/**/;
	Conveyor.sendItem(item, newDest);
}
} //******* PickOption End *******\\

```

### Fazer pull strategy nos processadores 
On exit do torrador send a message to estoque de cacau liberando mais 1 para entrar + entrar 4 iniciais
