FLAGS =  -I../include -framework GLUT -framework OpenGL -framework Cocoa pworld.o particle.o body.o collide_coarse.o collide_fine.o contacts.o core.o fgen.o joints.o pcontacts.o pfgen.o plinks.o random.o demos/main.o demos/app.o demos/timing.o

all:
	g++ -c body.cpp -I../include
	g++ -c collide_coarse.cpp -I../include
	g++ -c collide_fine.cpp -I../include
	g++ -c contacts.cpp -I../include
	g++ -c core.cpp -I../include
	g++ -c fgen.cpp -I../include
	g++ -c joints.cpp -I../include
	g++ -c particle.cpp -I../include
	g++ -c pcontacts.cpp -I../include
	g++ -c pfgen.cpp -I../include
	g++ -c plinks.cpp -I../include
	g++ -c pworld.cpp -I../include
	g++ -c random.cpp -I../include
	g++ -c world.cpp -I../include
	g++ -c demos/app.cpp -I../include -o demos/app.o
	g++ -c demos/main.cpp -I../include -o demos/main.o
	g++ -fasm-blocks -c demos/timing.cpp -I../include -o demos/timing.o
	g++ $(FLAGS) demos/ballistic/ballistic.cpp -o ../bin/ballistic.out
	g++ $(FLAGS) demos/bigballistic/bigballistic.cpp -o ../bin/bigballistic.out
	g++ $(FLAGS) demos/blob/blob.cpp -o ../bin/blob.out
	g++ $(FLAGS) demos/bridge/bridge.cpp -o ../bin/bridge.out
	g++ $(FLAGS) demos/explosion/explosion.cpp -o ../bin/explosion.out
	g++ $(FLAGS) demos/fireworks/fireworks.cpp -o ../bin/fireworks.out
	g++ $(FLAGS) demos/flightsim/flightsim.cpp -o ../bin/flightsim.out
	g++ $(FLAGS) demos/fracture/fracture.cpp -o ../bin/fracture.out
	g++ $(FLAGS) demos/platform/platform.cpp -o ../bin/platform.out
	g++ $(FLAGS) demos/ragdoll/ragdoll.cpp -o ../bin/ragdoll.out
	g++ $(FLAGS) demos/sailboat/sailboat.cpp -o ../bin/sailboat.out
