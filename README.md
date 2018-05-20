# economicdependent.h
///Cabecera de los Dependientes económicos
#ifndef ECONOMICDEPENDENT_H_INCLUDED
#define ECONOMICDEPENDENT_H_INCLUDED

/*** Cabeceras locales ***/
#include "name.h"

class EconomicDependent{
    private:
        Name name;
        int age;

    public:
        EconomicDependent();                                    ///Constructor base
        EconomicDependent(const EconomicDependent&);            /// Constructor Copia
        EconomicDependent(const Name&, int&);    ///Constructor Parametrizado

        /*** getters ***/
        Name getName();
        int getAge();

        /*** setters ***/
        void setName(const Name&);
        void setAge(const int&);

        std::string toString();     ///Imprime datos
};

#endif // ECONOMICDEPENDENT_H_INCLUDED
