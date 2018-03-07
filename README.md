#include<iostream>
#include<string>
#include<cmath>

using namespace std;

class CoffeGrender
{
public:
	string Getname()
	{
		return name;
	}
private:
	string name = "Apple";
};

class Switsgreender
{
public:
	bool chekworking()
	{
		bool voltageisormal = chekvoltage();
		if (voltageisormal == true)
		{
			if (this->working == false)
			{
				cout << "Автомат по продаже конфет выключен, пожалуйста включите прибор!" << endl;
				string chek;
				getline(cin, chek);
				if (chek == "on")
				{
					this->working = true;
					cout << "Машина работает, приятного апетита"<<endl;
				}
				else
				{
					this->working = false;
					cout << "Машина по прежнему выключена!!!Печеньки достанутся другому(((" << endl;
				}
			}
			else
				cout << "Поздравляю ты сломал ПО програма никогда не должна была заходить в это тёмное место" << endl;
		}
		else
			cout << "Полундра!!!P.S. что то пошло не так((!";
		return this->working;
	}
	void prize()
	{
		bool a = true;
		while (a)
		{
			cout << "Конфеты на любой вкус:" << endl;
			cout << "1.ТМ Рошен.............(код 1)" << endl;
			cout << "2.ТМ АВК...............(код 2)" << endl;
			cout << "3.ТМ Конти.............(код 3)" << endl;
			cout << "4.ТМ Свиточ............(код 4)" << endl;
			cout << "5.ТМ Любимов...........(код 5)" << endl;
			cout << endl;
			int choose;
			cout << "Сделайте свой выбор..." << endl;
			cin >> choose;
			switch (choose)
			{
			case(1):
			{
				cout << "Вы выбрали ТМ Рошен.Вот что у нас есть по етому пункту:" << endl;
				cout << "Рошен шоколад-1" << endl;
				cout << "Рошен мармелад-2" << endl;
				cout << "Рошен печенье-3" << endl;
				int p;
				cin >> p;
				if (p == 1)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->roshennumber < abs(f))
					{
						cout << "Конфет ТМ Рошен наличии всего " << this->roshennumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->roshennumber += (-abs(f));
				}
				if (p == 2)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->roshennumber < abs(f))
					{
						cout << "Конфет ТМ Рошен наличии всего " << this->roshennumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->roshennumber += (-abs(f));
				}
				if (p == 3)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->roshennumber < abs(f))
					{
						cout << "Конфет ТМ Рошен наличии всего " << this->roshennumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->roshennumber += (-abs(f));
				}
				break;
			}
			case(2):
			{
				cout << "Вы выбрали ТМ АВК.Вот что у нас есть по етому пункту:" << endl;
				cout << "АВК шоколад-1" << endl;
				cout << "АВК мармелад-2" << endl;
				cout << "АВК печенье-3" << endl;
				int k;
				cin >> k;
				if (k == 1)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->avknumber < abs(f))
					{
						cout << "Конфет ТМ АВК наличии всего " << this->avknumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->avknumber += (-abs(f));
				}
				if (k == 2)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->avknumber < abs(f))
					{
						cout << "Конфет ТМ АВК наличии всего " << this->avknumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->avknumber += (-abs(f));
				}
				if (k == 3)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->avknumber < abs(f))
					{
						cout << "Конфет ТМ АВК наличии всего " << this->avknumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->avknumber += (-abs(f));
				}
				break;
			}
			case(3):
			{
				cout << "Вы выбрали ТМ Конти.Вот что у нас есть по етому пункту:" << endl;
				cout << "Конти шоколад-1" << endl;
				cout << "Конти мармелад-2" << endl;
				cout << "Конти печенье-3" << endl;
				int g;
				cin >> g;
				if (g == 1)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->kontynumber < abs(f))
					{
						cout << "Конфет ТМ Конти наличии всего " << this->kontynumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->kontynumber += (-abs(f));
				}
				if (g == 2)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->kontynumber < abs(f))
					{
						cout << "Конфет ТМ Конти наличии всего " << this->kontynumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->kontynumber += (-abs(f));
				}
				if (g == 3)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->kontynumber < abs(f))
					{
						cout << "Конфет ТМ Конти наличии всего " << this->kontynumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->kontynumber += (-abs(f));
				}
				break;
			}
			case(4):
			{
				cout << "Вы выбрали ТМ Свиточ.Вот что у нас есть по етому пункту:" << endl;
				cout << "Свиточ шоколад-1" << endl;
				cout << "Свиточ мармелад-2" << endl;
				cout << "Свиточ печенье-3" << endl;
				int w;
				cin >> w;
				if (w == 1)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->svutochnumber < abs(f))
					{
						cout << "Конфет ТМ Свиточ наличии всего " << this->svutochnumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->svutochnumber += (-abs(f));
				}
				if (w == 2)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->svutochnumber < abs(f))
					{
						cout << "Конфет ТМ Свиточ наличии всего " << this->svutochnumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->svutochnumber += (-abs(f));
				}
				if (w == 3)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->svutochnumber < abs(f))
					{
						cout << "Конфет ТМ Свиточ наличии всего " << this->svutochnumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->svutochnumber += (-abs(f));
				}
				break;
			}
			case(5):
			{
				chekproduction();
				cout << "Вы выбрали ТМ Любимов.Вот что у нас есть по етому пункту:" << endl;
				cout << "Любимов шоколад-1" << endl;
				cout << "Любимов мармелад-2" << endl;
				cout << "Любимов печенье-3" << endl;
				int t;
				cin >> t;
				if (t == 1)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->lubemovnumber < abs(f))
					{
						cout << "Конфет ТМ Любимов наличии всего " << this->lubemovnumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->lubemovnumber += (-abs(f));
				}
				if (t == 2)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->lubemovnumber < abs(f))
					{
						cout << "Конфет ТМ Любимов наличии всего " << this->lubemovnumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->lubemovnumber += (-abs(f));
				}
				if (t == 3)
				{
					int f;
					cout << "Введите количество" << endl;
					cin >> f;
					if (this->lubemovnumber < abs(f))
					{
						cout << "Конфет ТМ Любимов наличии всего " << this->lubemovnumber << " штук.";
						cout << "Виберите другое кол-ство конфет";
					}
					else
						this->lubemovnumber += (-abs(f));
				}
				break;
			}
			}
			print();
			chekproduction();
			cout << "Завершить сеанс?" << endl;
			string question;
			cin >> question;
			//getline(cin, question);
			if (question == "yes" || question == "Yes")
			{
				a=false;
			}
			else
				cout << "Хороший выбор!!!";
		}
	}
	Switsgreender()
	{
		differentlyswits = 100;
		marka = "Sumsung";
		power = 2500;
		working = false;
	}
	~Switsgreender()
	{
		cout << "Вызвался деструктор" << endl;
	}
	void print()
	{
		cout << "Автомат " << marka << "  Мощность " << power <<  "  Статус  "<<working<<endl;
		cout << "Конфет ТМ Рошен в наличии " << roshennumber << endl;
		cout << "Конфет ТМ АВК в наличии " << avknumber << endl;
		cout << "Конфет ТМ Конти в наличии " << kontynumber << endl;
		cout << "Конфет ТМ Свиточ в наличии " << svutochnumber << endl;
		cout << "Конфет ТМ Любимов в наличии " << lubemovnumber << endl;
	}
	void inspectCoffeGrender()
	{
		cout << "Коффемашина марки " << coffe.Getname() << " Хороший апарат"<<endl;
	}
private:
	int differentlyswits;
	int roshennumber = 20;
	int avknumber = 20;
	int kontynumber = 20;
	int svutochnumber = 20;
	int lubemovnumber = 20;
	string marka;
	int power;
	bool working;
	bool chekvoltage()
	{
		return true;
	}
	void chekproduction()
	{
		if (this->roshennumber <= 5)
			this->roshennumber += 20;
		if (this->avknumber <= 3)
			this->avknumber += 10;
		if (this->kontynumber <= 4)
			this->kontynumber += 15;
		if (this->svutochnumber <= 4)
			this->svutochnumber += 15;
		if (this->lubemovnumber <= 4)
			this->lubemovnumber += 15;
	}
	CoffeGrender coffe;
};


class Sweets
{
public:
	virtual void nyamnyam() = 0;
};

class cake: public Sweets
{
public:
	void nyamnyam() override
	{
		cout << "Очень вкусний пирог..." << endl;
	}
};

class icecream : cake
{
public:
	void nyamnyam() override
	{
		cout << "Мороженое как частичка неба!" <<endl;
	}
};


class fruits : public Sweets
{
	void nyamnyam() override
	{
		cout << "Полезно очень вкусно..." << endl;
	}
};

class User
{
public:
	void nyamnyam(Sweets *weapon)
	{
		weapon->nyamnyam();
	}
};
int main()
{
	setlocale(LC_ALL, "ru");
	Switsgreender a;
	a.chekworking();
	a.prize();
	//a.print();
	a.inspectCoffeGrender();
	User user;
	fruits fruits;
	icecream cake;
	user.nyamnyam(&fruits);
	//user.nyamnyam(&cake);
	system("pause");
	return 0;
}
