<%*
	let name;
	if(tp.file.title.startsWith("Untitled")){
		name = await tp.user.random_femme() + " " + await tp.user.random_last();
		await tp.file.rename(name);
	}
_%>
---
tags:
- Random-NPC
aliases:
type: Randomized NPC
alignment:
race: <%await tp.user.random_race()%>
age:
age_group: <%await tp.user.random_age_group()%>
pronouns:
- She
- Her
- Hers
pronounced:
gender: Female
sexuality:  <%await tp.user.random_sexuality()%>
occupations:
location:
groups:
religions:
owns:
status: Alive
relationship_status:
classes:
subclasses:
level:
birthday:
style: NPC
family:
friends:
subordinates:
enemies:
image: "[[placeholder-NPC.webp]]"
icon: RaPerspectiveDiceRandom
---
>[!NPC-Wiki] `=this.file.name` `$= !dv.current().pronouns ? "" : "(" + dv.current().pronouns.join("/") + ")"`
> |             |                                                                        |
> |:----------- |:---------------------------------------------------------------------- |
> | **Aliases** | `$= !dv.current().aliases ? "None" : dv.current().aliases.join(", ") ` |
>`$= dv.paragraph(dv.func.embed(dv.current().image))`
>
> |                   |                                                                                                                                                          |
> |:----------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------- |
> | **Race**          | `$= !dv.current().race ? "N/A" : dv.current().race`                                                                                                      |
> | **Age**           | `$= !dv.current().age ? "N/A" : dv.current().age`                                                                                                        |
> | **Sexuality**     | `$= !dv.current().sexuality ? "N/A" : dv.current().sexuality`                                                                                            |
> | **Status**        | `$= !dv.current().status ? "N/A" : dv.current().status`                                                                                                  |
> | **Relationships** | `$= !dv.current().relationship_status ? "N/A" : dv.current().relationship_status`                                                                        |
> | **Class**         | `$= !dv.current().classes ? "N/A" : dv.current().classes.join(", ")` `$= !dv.current().subclasses ? "" : "(" + dv.current().subclasses.join(", ") + ")"` |
> | **Religions**     | `$= !dv.current().religions ? "None" : dv.current().religions.join(", ")`                                                                                |
> |                   |                                                                                                                                                          |
> | **Location**      | `$= !dv.current().location ? "N/A" : dv.current().location`                                                                                              |
> | **Origin**        | `$= !dv.current().origin ? "N/A" : dv.current().origin`                                                                                                  |
> | **Occupation**    | `$= !dv.current().occupations ? "None" : dv.current().occupations.join(", ")`                                                                            |
> | **Owns**          | `$= !dv.current().owns ? "N/A" : dv.current().owns.join(", ")`                                                                                           |
> | **Groups**        | `$= !dv.current().groups ? "None" : dv.current().groups.join(", ")`                                                        
# Description
>[!quote] Read To Players
>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vulputate iaculis dui, ut aliquet velit. Vivamus eu ornare sem. Quisque tincidunt, leo ac malesuada lobortis, dui nisl varius nunc, fermentum tincidunt velit nulla et ipsum. In mi nulla, hendrerit ac augue vel, porta porta urna. Nunc congue pretium eros, eu euismod arcu efficitur eget. Aliquam molestie neque in felis mollis, at accumsan enim tempus. Fusce rhoncus sollicitudin mauris, eget posuere risus tristique sagittis. Maecenas gravida dui dui, sit amet accumsan ipsum maximus vel. In tincidunt, elit nec tempor hendrerit, dui metus pulvinar ipsum, fringilla malesuada erat ex vitae mi. Sed non ullamcorper tellus, ac consectetur nunc. Sed lacus urna, accumsan quis nunc quis, scelerisque rutrum ipsum.
# Background
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vulputate iaculis dui, ut aliquet velit. Vivamus eu ornare sem. Quisque tincidunt, leo ac malesuada lobortis, dui nisl varius nunc, fermentum tincidunt velit nulla et ipsum. In mi nulla, hendrerit ac augue vel, porta porta urna. Nunc congue pretium eros, eu euismod arcu efficitur eget. Aliquam molestie neque in felis mollis, at accumsan enim tempus. Fusce rhoncus sollicitudin mauris, eget posuere risus tristique sagittis. Maecenas gravida dui dui, sit amet accumsan ipsum maximus vel. In tincidunt, elit nec tempor hendrerit, dui metus pulvinar ipsum, fringilla malesuada erat ex vitae mi. Sed non ullamcorper tellus, ac consectetur nunc. Sed lacus urna, accumsan quis nunc quis, scelerisque rutrum ipsum.
# Notes
- Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vulputate iaculis dui, ut aliquet velit. Vivamus eu ornare sem. Quisque tincidunt, leo ac malesuada lobortis, dui nisl varius nunc, 
- Sed non ullamcorper tellus, ac consectetur nunc. Sed lacus urna, accumsan quis nunc quis, scelerisque rutrum ipsum.


![[NPC-Banner.jpg|banner]]